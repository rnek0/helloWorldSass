# Working with Sass

1. D'abord il nous faut installer __dart SDK__ comme ceci par exemple pour Archlinux.  
```
yay -S dart
```  

2. Créer le fichier __pubspec.yaml__ comme ceci :  
```
name: my_project
dev_dependencies:
  sass: ^1.26.10
```  

3. Taper __pub get__  

4. Creer le fichier compile-sass.dart comme ceci :  

```dart
import 'dart:io';
import 'package:sass/sass.dart' as sass;

void main(List<String> arguments) {
  var result = sass.compile(arguments[0]);
  new File(arguments[1]).writeAsStringSync(result);
}
```  

5. On peut maintenat compiler pour créer nos fichiers css comme ceci

```bash
dart compile-sass.dart styles.scss styles.css
```  

> RTFM la doc sass library [sass compile function](https://pub.dev/documentation/sass/latest/sass/compile.html)  
> Apprendre sass [avec le guide](https://sass-lang.com/guide)  
> [Documentation sass](https://sass-lang.com/documentation)  

Enjoy it!

Update (05/03/23) :

* sdk: '>=2.12.0 <3.0.0' on pubspec.yaml
* dart pub get
```bash
❯ dart pub get
Resolving dependencies... 
Got dependencies!
```
* Compile
```bash
❯ dart compile-sass.dart styles.scss styles.css
```

[Test with minima ](blog/sass/README.md)

```bash
❯ dart compile-sass.dart peertube.scss peertube.css
```