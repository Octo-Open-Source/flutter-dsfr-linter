# Dsfr Lints

## Installation

Il est nécessaire d'ajouter le package `custom_lint` en tant que `dev_dependencies` dans le fichier `pubspec.yaml` du projet, ainsi que ce package `dsfr_lints`. Le package n'est actuellement pas publié sur pub.dev, mais il est possible d'ajouter la dépendance `dsfr_lints` dans le fichier pubspec.yaml en spécifiant l'url de ce repository et le tag d'une release. Exemple :

```
dev_dependencies:
  custom_lint:
  dsfr_lints:
    git:
      url: https://github.com/Octo-Open-Source/flutter-dsfr-linter.git
      ref: 0.1.0
```

Ensuite, il faut modifier le fichier `analysis_options.yaml` du projet pour ajouter custom_lint :

```
analyzer:
  plugins:
    - custom_lint
```

Plus d'informations sur le [README de custom_lint](https://github.com/invertase/dart_custom_lint).

## Ressources

- https://pub.dev/documentation/analyzer/latest/dart_ast_ast/
- https://github.com/invertase/dart_custom_lint
- https://charlescyt.github.io/create-your-own-lint-rules-with-custom-lint
