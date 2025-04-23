<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Juego Educativo Secundaria</title>
  <style>
    :root {
      --bg-light: #f9fafc;
      --bg-dark: #1e1e2f;
      --text-light: #1e1e2f;
      --text-dark: #f9fafc;
      --primary: #4f46e5;
      --secondary: #6366f1;
      --correct: #16a34a;
      --incorrect: #dc2626;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: var(--bg-light);
      color: var(--text-light);
      margin: 0;
      padding: 2rem;
      transition: all 0.3s ease-in-out;
    }
    body.dark-mode {
      background: var(--bg-dark);
      color: var(--text-dark);
    }
    .container {
      max-width: 800px;
      margin: auto;
      background: white;
      border-radius: 1rem;
      padding: 2rem;
      box-shadow: 0 4px 20px rgba(0,0,0,0.1);
      transition: background 0.3s ease;
    }
    body.dark-mode .container {
      background: #2d2e4a;
    }
    h1, h2 {
      text-align: center;
    }
    select, button {
      display: block;
      width: 100%;
      margin-top: 1rem;
      padding: 1rem;
      font-size: 1rem;
      border-radius: 0.5rem;
      border: 2px solid var(--primary);
      background: white;
      transition: background 0.3s ease;
    }
    body.dark-mode select, body.dark-mode button {
      background: #3b3c5c;
      color: white;
      border-color: var(--secondary);
    }
    button:hover {
      background: var(--primary);
      color: white;
    }
    .question-box {
      margin-top: 2rem;
    }
    .option {
      margin-top: 0.5rem;
      padding: 0.75rem;
      border: 2px solid #ccc;
      border-radius: 0.5rem;
      cursor: pointer;
      background: #f9f9f9;
      transition: background 0.3s ease;
    }
    .option:hover {
      background: var(--secondary);
      color: white;
    }
    .option.correct {
      background: var(--correct);
      color: white;
    }
    .option.incorrect {
      background: var(--incorrect);
      color: white;
    }
    .score {
      margin-top: 1rem;
      text-align: center;
      font-weight: bold;
    }
    .dark-toggle {
      position: absolute;
      top: 1rem;
      right: 1rem;
      background: transparent;
      border: none;
      cursor: pointer;
      font-size: 1.5rem;
    }
  </style>
</head>
<body>
  <button class="dark-toggle" onclick="toggleDarkMode()">🌓</button>
  <div class="container">
    <h1>Juego Educativo</h1>

    <h2>Selecciona Grado, Asignatura y Dificultad</h2>
    <select id="grade">
      <option value="9">Grado 9</option>
      <option value="10">Grado 10</option>
      <option value="11">Grado 11</option>
      <option value="12">Grado 12</option>
    </select>
    <select id="subject">
      <option value="Matemáticas">Matemáticas</option>
      <option value="Ciencias">Ciencias</option>
      <option value="Historia">Historia</option>
      <option value="Literatura">Literatura</option>
    </select>
    <select id="difficulty">
      <option value="Fácil">Fácil</option>
      <option value="Medio">Medio</option>
      <option value="Difícil">Difícil</option>
    </select>
    <button onclick="startGame()">Iniciar Juego</button>

    <div class="question-box" id="questionBox" style="display: none;">
      <h2 id="question"></h2>
      <div id="options"></div>
      <div class="score" id="score"></div>
    </div>
  </div>

  <script>
    const questions = {
  "Matemáticas": {
    "9": {
      "Fácil": [
        { question: "¿Cuánto es 5 + 3?", options: ["6", "7", "8", "9"], answer: "8" },
        { question: "¿Cuál es el valor de x en: x + 4 = 10?", options: ["5", "6", "7", "8"], answer: "6" },
        { question: "¿Cuánto es 3²?", options: ["6", "9", "12", "3"], answer: "9" }
      ],
      "Medio": [
        { question: "¿Cuánto es (3+5) × 2?", options: ["10", "14", "16", "12"], answer: "16" },
        { question: "¿Cuánto es 12 ÷ 3 + 2?", options: ["6", "5", "4", "3"], answer: "6" }
      ],
      "Difícil": [
        { question: "¿Cuál es la raíz cuadrada de 144?", options: ["10", "12", "14", "16"], answer: "12" },
        { question: "¿Qué es 2³ + 4²?", options: ["24", "20", "18", "16"], answer: "24" }
      ]
    },
    "10": {
      "Fácil": [
        { question: "¿Qué es 7 × 6?", options: ["42", "36", "48", "40"], answer: "42" }
      ],
      "Medio": [
        { question: "Resuelve: 15 - 3 × 2", options: ["6", "9", "12", "3"], answer: "9" }
      ],
      "Difícil": [
        { question: "¿Cuánto es (5 + 3)²?", options: ["64", "49", "36", "81"], answer: "64" }
      ]
    }
  },
  "Ciencias": {
    "9": {
      "Fácil": [
        { question: "¿Cuál es el estado líquido del agua?", options: ["Hielo", "Vapor", "Agua", "Niebla"], answer: "Agua" },
        { question: "¿Qué planeta es conocido como el planeta rojo?", options: ["Marte", "Venus", "Júpiter", "Saturno"], answer: "Marte" }
      ]
    },
    "10": {
      "Fácil": [
        { question: "¿Qué órgano del cuerpo humano bombea sangre?", options: ["Pulmones", "Riñones", "Hígado", "Corazón"], answer: "Corazón" }
      ],
      "Medio": [
        { question: "¿Qué gas es necesario para la respiración humana?", options: ["Nitrógeno", "Oxígeno", "Dióxido de carbono", "Hidrógeno"], answer: "Oxígeno" }
      ],
      "Difícil": [
        { question: "¿Cuál es la fórmula química del agua?", options: ["CO2", "H2O", "NaCl", "O2"], answer: "H2O" }
      ]
    }
  },
  "Historia": {
    "9": {
      "Fácil": [
        { question: "¿En qué año ocurrió la independencia de México?", options: ["1810", "1821", "1800", "1850"], answer: "1810" },
        { question: "¿Quién descubrió América?", options: ["Simón Bolívar", "Cristóbal Colón", "Hernán Cortés", "Benito Juárez"], answer: "Cristóbal Colón" }
      ],
      "Medio": [
        { question: "¿Qué civilización construyó las pirámides de Egipto?", options: ["Aztecas", "Mayas", "Egipcios", "Incas"], answer: "Egipcios" }
      ],
      "Difícil": [
        { question: "¿Cuál fue la principal causa de la Primera Guerra Mundial?", options: ["Crisis económica", "Asesinato del archiduque", "Colonialismo", "Religión"], answer: "Asesinato del archiduque" }
      ]
    },
    "10": {
      "Fácil": [
        { question: "¿Qué civilización prehispánica habitó en México central?", options: ["Mayas", "Incas", "Aztecas", "Egipcios"], answer: "Aztecas" }
      ],
      "Medio": [
        { question: "¿En qué siglo ocurrió la Revolución Francesa?", options: ["XV", "XVI", "XVIII", "XIX"], answer: "XVIII" }
      ],
      "Difícil": [
        { question: "¿Qué tratado puso fin a la Primera Guerra Mundial?", options: ["Versalles", "Guadalupe Hidalgo", "Tordesillas", "París"], answer: "Versalles" }
      ]
    }
  },
  "Literatura": {
    "9": {
      "Fácil": [
        { question: "¿Quién escribió Don Quijote de la Mancha?", options: ["Gabriel García Márquez", "Miguel de Cervantes", "Pablo Neruda", "Jorge Luis Borges"], answer: "Miguel de Cervantes" },
        { question: "¿Qué es una metáfora?", options: ["Una comparación sin 'como'", "Un adjetivo", "Un verbo", "Una exageración"], answer: "Una comparación sin 'como'" }
      ],
      "Medio": [
        { question: "¿Qué tipo de texto es una fábula?", options: ["Narrativo", "Argumentativo", "Lírico", "Expositivo"], answer: "Narrativo" }
      ],
      "Difícil": [
        { question: "¿Qué poeta escribió '20 poemas de amor y una canción desesperada'?", options: ["Bécquer", "Pablo Neruda", "Lorca", "Rubén Darío"], answer: "Pablo Neruda" }
      ]
    },
    "10": {
      "Fácil": [
        { question: "¿Qué es un poema?", options: ["Una pintura", "Un texto lírico", "Una novela", "Un ensayo"], answer: "Un texto lírico" }
      ],
      "Medio": [
        { question: "¿Qué autor escribió 'Cien años de soledad'?", options: ["Julio Cortázar", "Mario Vargas Llosa", "Gabriel García Márquez", "Isabel Allende"], answer: "Gabriel García Márquez" }
      ],
      "Difícil": [
        { question: "¿Cuál de los siguientes autores pertenece al realismo mágico?", options: ["Borges", "García Márquez", "Neruda", "Darío"], answer: "García Márquez" }
      ]
    }
  }
};

    let currentQuestion = 0;
    let currentData = [];
    let score = 0;

    function startGame() {
      const grade = document.getElementById("grade").value;
      const subject = document.getElementById("subject").value;
      const difficulty = document.getElementById("difficulty").value;

      if (
        questions[subject] &&
        questions[subject][grade] &&
        questions[subject][grade][difficulty]
      ) {
        currentData = questions[subject][grade][difficulty];
        currentQuestion = 0;
        score = 0;
        document.getElementById("score").innerText = "";
        document.getElementById("questionBox").style.display = "block";
        showQuestion();
      } else {
        alert("No hay preguntas disponibles para esta combinación.");
      }
    }

    function showQuestion() {
      const q = currentData[currentQuestion];
      document.getElementById("question").innerText = q.question;
      const optionsBox = document.getElementById("options");
      optionsBox.innerHTML = "";
      q.options.forEach(option => {
        const div = document.createElement("div");
        div.className = "option";
        div.innerText = option;
        div.onclick = () => selectAnswer(div, option);
        optionsBox.appendChild(div);
      });
    }

    function selectAnswer(div, selected) {
      const correct = currentData[currentQuestion].answer;
      const allOptions = document.querySelectorAll(".option");
      allOptions.forEach(opt => opt.onclick = null);
      if (selected === correct) {
        score++;
        div.classList.add("correct");
      } else {
        div.classList.add("incorrect");
        allOptions.forEach(opt => {
          if (opt.innerText === correct) opt.classList.add("correct");
        });
      }
      setTimeout(() => {
        currentQuestion++;
        if (currentQuestion < currentData.length) {
          showQuestion();
        } else {
          document.getElementById("score").innerText = `Puntaje final: ${score} / ${currentData.length}`;
        }
      }, 1000);
    }

    function toggleDarkMode() {
      document.body.classList.toggle("dark-mode");
    }
  </script>
</body>
</html>
