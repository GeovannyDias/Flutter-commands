# Comandos de Flutter, Dart, FVM

## Flutter
* *https://flutter.dev/docs/get-started/install/windows*

```
Agregar a PATH:
C:\src\flutter\bin

flutter doctor
flutter upgrade

```
## Dart

```
Si ya se tiene instalado Flutter se debe agregar el PATH en las varibles de entorno:

C:\src\flutter\bin\cache\dart-sdk\bin

dart --version
pub --version

```

## Flutter Version Management
* *https://github.com/leoafarias/fvm*

```
Install Dart.
Activate Fvm:

Para instalar FVM, en una terminal correr el siguiente comando:

pub global activate fvm

es recomendable que se instale en los directorios de Flutter para poder agregar el PATH facilmente:

flutter pub global activate fvm

Agregar el PATH de FVM:

C:\src\flutter\.pub-cache\bin

fvm help
fvm version
fvm install master

fvm use <version>
fvm install 1.20.0

fvm use <version> --global
fvm use 1.20.0 --global

fvm use <version> --force
fvm remove <version>

fvm list
fvm releases
dev, beta and stable, master

Available commands:
  config     Set configuration for FVM
  flutter    Proxies Flutter Commands
  install    Installs Flutter SDK Version
  list       Lists installed Flutter SDK Version
  releases   Lists Flutter SDK releases.
  remove     Removes Flutter SDK Version
  use        Which Flutter SDK Version you would like to use
  version    Prints the currently-installed version of FVM


Desinstalar:

pub global deactivate fvm
flutter pub global deactivate fvm

For instance, to run the flutter run with a given Flutter SDK version just call the following.
FVM will recursively try for a version in a parent directory.

fvm flutter run

This syntax works also for commands with parameters.
The following command will call flutter build for a selected flavor and target.

fvm flutter build aab --release --flavor prod -t lib/main_prod.dart

Troubleshooting:

On Windows make sure you are running as an administrator
If you get errors with messages invalid kernel binary or 
invalid sdk hash it means you activated fvm using flutter pub global activate fvm.
Only activate fvm using pub global activate fvm.

pub cache repair

```




