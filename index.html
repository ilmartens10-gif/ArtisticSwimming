<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meine Quiz-Welt</title>
    <style>
        /* --- DESIGN (CSS) --- */
        * {
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: #f4f7f6;
            color: #333;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            background-color: #4A90E2;
            color: white;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        main {
            flex: 1;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .quiz-card {
            background: white;
            border-radius: 12px;
            padding: 30px;
            max-width: 500px;
            width: 100%;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        .question {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 20px;
        }

        .options-grid {
            display: grid;
            gap: 10px;
        }

        .btn {
            background-color: #f0f0f0;
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            padding: 12px 15px;
            font-size: 1rem;
            cursor: pointer;
            transition: all 0.2s ease;
            text-align: left;
        }

        .btn:hover {
            background-color: #e2e8f0;
            border-color: #cbd5e1;
        }

        .btn.correct {
            background-color: #86efac;
            border-color: #22c55e;
            color: #14532d;
        }

        .btn.incorrect {
            background-color: #fca5a5;
            border-color: #ef4444;
            color: #7f1d1d;
        }

        .next-btn {
            margin-top: 20px;
            background-color: #4A90E2;
            color: white;
            border: none;
            width: 100%;
            padding: 12px;
            border-radius: 8px;
            font-weight: bold;
            cursor: pointer;
            display: none;
        }

        .next-btn:hover {
            background-color: #357abd;
        }

        .results {
            text-align: center;
        }

        .results h2 {
            margin-bottom: 15px;
        }

        footer {
            text-align: center;
            padding: 1rem;
            font-size: 0.9rem;
            color: #666;
        }
    </style>
</head>
<body>

    <header>
        <h1>🎯 Das Ultimative Quiz</h1>
        <p>Teste dein Wissen in verschiedenen Bereichen!</p>
    </header>

    <main>
        <div class="quiz-card" id="quiz-box">
            <div id="question-container">
                <div class="question" id="question">Frage wird geladen...</div>
                <div class="options-grid" id="answer-buttons">
                    </div>
            </div>
            <button id="next-btn" class="next-btn">Nächste Frage</button>
            <div id="result-container" class="results" style="display: none;">
                <h2>Ergebnis</h2>
                <p id="score-text"></p>
                <button class="btn" onclick="restartQuiz()" style="margin-top: 15px; text-align: center;">Nochmal spielen</button>
            </div>
        </div>
    </main>

    <footer>
        <p>&copy; 2026 Quiz-Webseite. Erstellt für tüftlerische Köpfe.</p>
    </footer>

    <script>
        /* --- LOGIK (JAVASCRIPT) --- */

        // Hier kannst du beliebig viele Fragen hinzufügen!
        const questions = [
            {
                question: "Welches ist das flächenmäßig größte Land der Erde?",
                answers: [
                    { text: "Kanada", correct: false },
                    { text: "Russland", correct: true },
                    { text: "China", correct: false },
                    { text: "USA", correct: false }
                ]
            },
            {
                question: "Wie viele Planeten hat unser Sonnensystem?",
                answers: [
                    { text: "7", correct: false },
                    { text: "8", correct: true },
                    { text: "9", correct: false },
                    { text: "10", correct: false }
                ]
            },
            {
                question: "Welche Farbe hat ein Smaragd?",
                answers: [
                    { text: "Blau", correct: false },
                    { text: "Rot", correct: false },
                    { text: "Grün", correct: true },
                    { text: "Gelb", correct: false }
                ]
            }
        ];

        const questionElement = document.getElementById('question');
        const answerButtonsElement = document.getElementById('answer-buttons');
        const nextButton = document.getElementById('next-btn');
        const resultContainer = document.getElementById('result-container');
        const questionContainer = document.getElementById('question-container');
        const scoreText = document.getElementById('score-text');

        let currentQuestionIndex = 0;
        let score = 0;

        function startQuiz() {
            currentQuestionIndex = 0;
            score = 0;
            resultContainer.style.display = 'none';
            questionContainer.style.display = 'block';
            nextButton.innerText = 'Nächste Frage';
            showQuestion();
        }

        function showQuestion() {
            resetState();
            let currentQuestion = questions[currentQuestionIndex];
            questionElement.innerText = `${currentQuestionIndex + 1}. ${currentQuestion.question}`;

            currentQuestion.answers.forEach(answer => {
                const button = document.createElement('button');
                button.innerText = answer.text;
                button.classList.add('btn');
                if (answer.correct) {
                    button.dataset.correct = answer.correct;
                }
                button.addEventListener('click', selectAnswer);
                answerButtonsElement.appendChild(button);
            });
        }

        function resetState() {
            nextButton.style.display = 'none';
            while (answerButtonsElement.firstChild) {
                answerButtonsElement.removeChild(answerButtonsElement.firstChild);
            }
        }

        function selectAnswer(e) {
            const selectedButton = e.target;
            const isCorrect = selectedButton.dataset.correct === "true";
            
            if (isCorrect) {
                selectedButton.classList.add('correct');
                score++;
            } else {
                selectedButton.classList.add('incorrect');
            }

            Array.from(answerButtonsElement.children).forEach(button => {
                if (button.dataset.correct === "true") {
                    button.classList.add('correct');
                }
                button.disabled = true;
            });

            if (questions.length > currentQuestionIndex + 1) {
                nextButton.style.display = 'block';
            } else {
                nextButton.innerText = 'Ergebnis anzeigen';
                nextButton.style.display = 'block';
            }
        }

        function showScore() {
            resetState();
            questionContainer.style.display = 'none';
            resultContainer.style.display = 'block';
            scoreText.innerText = `Du hast ${score} von ${questions.length} Fragen richtig beantwortet!`;
        }

        function handleNextButton() {
            currentQuestionIndex++;
            if (currentQuestionIndex < questions.length) {
                showQuestion();
            } else {
                showScore();
            }
        }

        nextButton.addEventListener('click', () => {
            if (currentQuestionIndex < questions.length) {
                handleNextButton();
            } else {
                startQuiz();
            }
        });

        function restartQuiz() {
            startQuiz();
        }

        // Quiz beim Laden der Seite starten
        startQuiz();
    </script>
</body>
</html>
