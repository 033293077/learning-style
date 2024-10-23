<!DOCTYPE html>
<html lang="he">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>שאלון סגנון למידה</title>
    <style>
        .question {
            display: none;
        }
        .active {
            display: block;
        }
    </style>
</head>
<body>
    <h1>בחן את סגנון הלמידה שלך</h1>

    <form id="learning-style-quiz">
        <div class="question active" id="question1">
            <h2>כיצד אתה מעדיף לקבל מידע חדש?</h2>
            <input type="checkbox" id="visual" name="learning-style" value="visual">
            <label for="visual">באמצעות דימויים, גרפים, ומפות</label><br>
            <input type="checkbox" id="auditory" name="learning-style" value="auditory">
            <label for="auditory">דרך הרצאות או הקלטות שמע</label><br>
            <input type="checkbox" id="kinesthetic" name="learning-style" value="kinesthetic">
            <label for="kinesthetic">אני מעדיף להתנסות ולהיות בתנועה תוך כדי למידה</label><br>
            <input type="checkbox" id="textual" name="learning-style" value="textual">
            <label for="textual">דרך קריאת טקסטים וסיכום</label><br><br>
            <button type="button" onclick="nextQuestion(1)">הבא</button>
        </div>

        <div class="question" id="question2">
            <h2>מהי הדרך האידיאלית שלך ללמידה?</h2>
            <input type="checkbox" id="independent" name="learning-approach" value="independent">
            <label for="independent">אני מעדיף לעבוד לבד בקצב שלי</label><br>
            <input type="checkbox" id="social" name="learning-approach" value="social">
            <label for="social">אני נהנה מלמידה קבוצתית ושיתוף פעולה עם אחרים</label><br>
            <input type="checkbox" id="goal-oriented" name="learning-approach" value="goal-oriented">
            <label for="goal-oriented">אני צריך מטרה ברורה ומשימות מוגדרות מראש</label><br>
            <input type="checkbox" id="curious" name="learning-approach" value="curious">
            <label for="curious">אני נהנה לחקור וללמוד נושאים שונים בגמישות רבה</label><br><br>
            <button type="button" onclick="nextQuestion(2)">הבא</button>
        </div>

        <!-- המשך השאלות -->

    </form>

    <script>
        function nextQuestion(currentQuestion) {
            document.getElementById('question' + currentQuestion).style.display = 'none';
            document.getElementById('question' + (currentQuestion + 1)).style.display = 'block';
        }
    </script>
</body>
</html>

