import 'package:flutter/material.dart';

void main() {
  runApp(const MainApp());
}

class MainApp extends StatelessWidget {
  const MainApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          backgroundColor: Colors.green,
          centerTitle: true,
          title: const Text(
            'Atividades',
            style: TextStyle(
              fontFamily: 'Quicksand',
              fontSize: 34,
            ),
          ),
        ),
        body: const Column(
          children: [
            // Atividade que vai acontecer
            Row(
              children: [
                Icon(Icons.check_box, color: Colors.blue),
                SizedBox(width: 20),
                Text(
                  'Estudar para prova de matemática.',
                  style: TextStyle(
                    color: Colors.blue,
                    fontFamily: 'Quicksand',
                    fontSize: 26,
                  ),
                ),
                Expanded(
                  child: Align(
                    alignment: Alignment.centerRight,
                    child: Text(
                      '16/08/2024',
                      style: TextStyle(
                        color: Colors.blue,
                        fontFamily: 'Quicksand',
                        fontSize: 22,
                      ),
                    ),
                  ),
                ),
              ],
            ),
            SizedBox(height: 10),
            
            // Atividade que já aconteceu
            Row(
              children: [
                Icon(Icons.check_box, color: Colors.black),
                SizedBox(width: 20),
                Text(
                  'Campeonato de futebol.',
                  style: TextStyle(
                    color: Colors.black,
                    fontFamily: 'Quicksand',
                    fontSize: 26,
                  ),
                ),
                Expanded(
                  child: Align(
                    alignment: Alignment.centerRight,
                    child: Text(
                      '14/08/2024',
                      style: TextStyle(
                        color: Colors.black,
                        fontFamily: 'Quicksand',
                        fontSize: 22,
                      ),
                    ),
                  ),
                ),
              ],
            ),
            SizedBox(height: 10),
            
            // Atividade que vai acontecer e está marcada como feita
            Row(
              children: [
                Icon(Icons.check_box, color: Colors.green),
                SizedBox(width: 20),
                Text(
                  'Festa da Joana',
                  style: TextStyle(
                    color: Colors.green,
                    fontFamily: 'Quicksand',
                    fontSize: 26,
                  ),
                ),
                Expanded(
                  child: Align(
                    alignment: Alignment.centerRight,
                    child: Text(
                      '23/08/2024',
                      style: TextStyle(
                        color: Colors.green,
                        fontFamily: 'Quicksand',
                        fontSize: 22,
                      ),
                    ),
                  ),
                ),
              ],
            ),
            SizedBox(height: 10),
            
            // Atividade cancelada com linethrough
            Row(
              children: [
                Icon(Icons.cancel, color: Colors.red),
                SizedBox(width: 20),
                Text(
                  'Viagem para praia',
                  style: TextStyle(
                    color: Colors.red,
                    fontFamily: 'Quicksand',
                    fontSize: 26,
                    decoration: TextDecoration.lineThrough,
                  ),
                ),
                Expanded(
                  child: Align(
                    alignment: Alignment.centerRight,
                    child: Text(
                      '01/09/2024',
                      style: TextStyle(
                        color: Colors.red,
                        fontFamily: 'Quicksand',
                        fontSize: 22,
                        decoration: TextDecoration.lineThrough,
                      ),
                    ),
                  ),
                ),
              ],
            ),
          ],
        ),
      ),
    );
  }
}
