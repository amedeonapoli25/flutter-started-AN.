# Flutter Getting Started - Amedeo Napolitano

Primo esercizio del corso di Enterprise Mobile Application Development.
Il progetto conserva l'app contatore generata da Flutter e personalizza il
titolo della schermata iniziale con **Amedeo Napolitano**.

## Modifica effettuata

In `lib/main.dart`:

- `MaterialApp.title` contiene il nome dell'autore.
- `MyHomePage.title` contiene lo stesso nome, mostrato nella barra superiore
  tramite `AppBar.title`.

Il pulsante `+` incrementa il contatore tramite `setState()`.

## Requisiti

- Flutter 3.47.7 stable con Dart 3.13.5 o una versione compatibile.
- Xcode su macOS per eseguire la versione iOS.
- Android Studio e Android SDK per eseguire la versione Android.

## Avvio

Aprire un terminale nella cartella del progetto, con Flutter nel PATH:

```sh
flutter pub get
flutter devices
flutter run -d ID_DISPOSITIVO
```

Sostituire `ID_DISPOSITIVO` con l'identificativo mostrato da `flutter devices`.

Per iPhone fisico: collegare e autorizzare il dispositivo, abilitare la
Modalità sviluppatore e configurare il proprio team di firma in Xcode.
Aprire il progetto iOS con:

```sh
open ios/Runner.xcworkspace
```

In Xcode selezionare Runner > Signing & Capabilities, abilitare
Automatically manage signing e scegliere il proprio Team. Se necessario,
impostare un Bundle Identifier univoco.

## Verifica del codice

```sh
flutter analyze
flutter test
```

Il test generato da Flutter verifica che il pulsante `+` incrementi il contatore.
La prova sul telefono fisico va effettuata separatamente.

## Consegna

- Link alla repository GitHub pubblica con il progetto completo.
- Screenshot originale dell'app in esecuzione su iPhone fisico, con
  **Amedeo Napolitano** leggibile.

Una cattura dal simulatore è utile per la verifica preliminare, ma la consegna
richiede lo screenshot dal telefono fisico.

I file temporanei, le cartelle di compilazione e le configurazioni locali
escluse da `.gitignore` non sono necessari per ricostruire il progetto.

## Documentazione ufficiale

- [Installazione Flutter](https://docs.flutter.dev/install/manual)
- [Configurazione iOS](https://docs.flutter.dev/platform-integration/ios/setup)
- [Configurazione Android](https://docs.flutter.dev/platform-integration/android/setup)
