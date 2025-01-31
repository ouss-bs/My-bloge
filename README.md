# My-bloge
Simple blog 
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مدونتي</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>مدونتي</h1>
    </header>

    <main>
        <article class="post">
            <h2><a href="post.html">عنوان المقال الأول</a></h2>
            <p>هذا نص مختصر عن المقال الأول. اضغط على العنوان لقراءة المزيد...</p>
        </article>

        <article class="post">
            <h2><a href="post.html">عنوان المقال الثاني</a></h2>
            <p>هذا نص مختصر عن المقال الثاني. اضغط على العنوان لقراءة المزيد...</p>
        </article>
    </main>

</body>
</html><!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مقال - مدونتي</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>مدونتي</h1>
    </header>

    <main>
        <article>
            <h2>عنوان المقال الأول</h2>
            <p>هذا هو نص المقال بالكامل. يمكنك إضافة محتوى هنا.</p>
            <a href="index.html">العودة إلى الصفحة الرئيسية</a>
        </article>
    </main>

</body>
</html>body {
    font-family: Arial, sans-serif;
    direction: rtl;
    text-align: right;
    margin: 0;
    padding: 0;
}

header {
    background: #333;
    color: white;
    text-align: center;
    padding: 15px;
}

main {
    width: 80%;
    margin: 20px auto;
}

.post {
    border-bottom: 1px solid #ddd;
    padding: 10px 0;
}

.post h2 a {
    text-decoration: none;
    color: #007BFF;
}

.post h2 a:hover {
    text-decoration: underline;
}document.addEventListener("DOMContentLoaded", function() {
    let posts = document.querySelectorAll(".post h2 a");
    posts.forEach(post => {
        post.addEventListener("click", function() {
            alert("جارٍ تحميل المقال...");
        });
    });
});
