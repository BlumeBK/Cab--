# Cab-ren
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:my_car_app/login/login_screen.dart';
/*import 'package:firebase_core/firebase_core.dart';
import 'firebase_options.dart'; */

Future<void> main() async {

  /*await Firebase.initializeApp(
    options: DefaultFirebaseOptions.currentPlatform,
  ); */
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'My_Car_App',
      theme: ThemeData(
        primarySwatch: Colors.blue,
        visualDensity: VisualDensity.adaptivePlatformDensity,
        textTheme: GoogleFonts.mulishTextTheme(),
      ),

      debugShowCheckedModeBanner: false,
      home: const LoginScreen(),
    );
  }
}
