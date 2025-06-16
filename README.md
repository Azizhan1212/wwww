<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Overwatch | Главная</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <header>
        <div class="logo">
            <img src="images/logos/overwatch-logo.png" alt="Overwatch Logo">
        </div>
        <nav>
            <ul>
                <li class="active"><a href="index.html">Главная</a></li>
                <li><a href="heroes.html">Герои</a></li>
                <li><a href="news.html">Новости</a></li>
                <li><a href="#about">О проекте</a></li>
            </ul>
        </nav>
        <div class="auth">
            <button class="login-btn"><i class="fas fa-user"></i> Войти</button>
        </div>
    </header>
    <section class="hero-banner">
        <div class="banner-content">
            <h1>Overwatch 2</h1>
            <p>Присоединяйтесь к битве за будущее</p>
            <button class="cta-button">Узнать больше</button>
        </div>
    </section>
    <section class="featured-heroes">
        <h2>Популярные герои</h2>
        <div class="hero-grid">
            <div class="hero-card">
                <img src="images/heroes/tracer.jpg" alt="Tracer">
                <h3>Tracer</h3>
                <p>Атакующий</p>
            </div>
            <div class="hero-card">
                <img src="images/heroes/reinhardt.jpg" alt="Reinhardt">
                <h3>Reinhardt</h3>
                <p>Танк</p>
            </div>
            <div class="hero-card">
                <img src="images/heroes/mercy.jpg" alt="Mercy">
                <h3>Mercy</h3>
                <p>Поддержка</p>
            </div>
        </div>
    </section>
    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>Overwatch</h3>
                <p>Официальный фан-сайт</p>
            </div>
            <div class="footer-section">
                <h3>Ссылки</h3>
                <ul>
                    <li><a href="#">Blizzard Entertainment</a></li>
                    <li><a href="#">Официальный сайт</a></li>
                    <li><a href="#">Форум</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>Контакты</h3>
                <p>info@overwatch-fan.ru</p>
                <div class="social-icons">
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-discord"></i></a>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2023 Overwatch Fan Site. Неофициальный проект.</p>
        </div>
    </footer>
   <script src="js/main.js"></script>
</body>
</html>
/* Основные стили */
:root {
    --primary-color: #f99e1a;
    --secondary-color: #218ffe;
    --dark-color: #0e1621;
    --light-color: #f5f5f5;
    --overwatch-blue: #00a1e6;
    --overwatch-orange: #f99e1a;
}
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}
body {
    background-color: var(--dark-color);
    color: var(--light-color);
    line-height: 1.6;
}
a {
    text-decoration: none;
    color: var(--light-color);
}
/* Шапка */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 5%;
    background-color: rgba(14, 22, 33, 0.9);
    position: fixed;
    width: 100%;
    z-index: 1000;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
}
.logo img {
    height: 40px;
}
nav ul {
    display: flex;
    list-style: none;
}
nav ul li {
    margin: 0 1rem;
    position: relative;
}
nav ul li a {
    padding: 0.5rem 1rem;
    font-weight: bold;
    transition: color 0.3s;
}
nav ul li a:hover {
    color: var(--primary-color);
}
nav ul li.active a {
    color: var(--primary-color);
    border-bottom: 2px solid var(--primary-color);
}
.auth .login-btn {
    background-color: var(--primary-color);
    color: var(--dark-color);
    border: none;
    padding: 0.5rem 1.5rem;
    border-radius: 4px;
    font-weight: bold;
    cursor: pointer;
    transition: all 0.3s;
}
.auth .login-btn:hover {
    background-color: #e68a00;
    transform: translateY(-2px);
}
/* Баннер */
.hero-banner {
    height: 100vh;
    background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                url('../images/overwatch-banner.jpg') no-repeat center center/cover;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding-top: 80px;
}
.banner-content h1 {
    font-size: 4rem;
    margin-bottom: 1rem;
    color: var(--overwatch-blue);
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}
.banner-content p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
}
.cta-button {
    background-color: var(--overwatch-orange);
    color: var(--dark-color);
    border: none;
    padding: 1rem 2.5rem;
    font-size: 1.2rem;
    font-weight: bold;
    border-radius: 4px;
    cursor: pointer;
    transition: all 0.3s;
}
.cta-button:hover {
    background-color: #e68a00;
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(249, 158, 26, 0.4);
}
/* Карточки героев */
.featured-heroes {
    padding: 5rem 10%;
    text-align: center;
}
.featured-heroes h2 {
    font-size: 2.5rem;
    margin-bottom: 3rem;
    color: var(--overwatch-blue);
}
.hero-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}
.hero-card {
    background-color: rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s, box-shadow 0.3s;
}
.hero-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0, 161, 230, 0.3);
}
.hero-card img {
    width: 100%;
    height: 300px;
    object-fit: cover;
}
.hero-card h3 {
    padding: 1rem;
    font-size: 1.5rem;
    color: var(--primary-color);
}
.hero-card p {
    padding: 0 1rem 1.5rem;
    color: var(--light-color);
}
/* Подвал */
footer {
    background-color: #0a1019;
    padding: 3rem 10% 1rem;
}
.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin-bottom: 2rem;
}
.footer-section h3 {
    color: var(--primary-color);
    margin-bottom: 1rem;
    font-size: 1.2rem;
}
.footer-section ul {
    list-style: none;
}
.footer-section ul li {
    margin-bottom: 0.5rem;
}
.social-icons {
    margin-top: 1rem;
}
.social-icons a {
    display: inline-block;
    margin-right: 1rem;
    font-size: 1.5rem;
    transition: color 0.3s;
}
.social-icons a:hover {
    color: var(--primary-color);
}

.footer-bottom {
    text-align: center;
    padding-top: 1.5rem;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    font-size: 0.9rem;
    color: rgba(255, 255, 255, 0.6);
}
/* Адаптивность */
@media (max-width: 768px) {
    header {
        flex-direction: column;
        padding: 1rem;
    }
    nav ul {
        margin: 1rem 0;
    }
    .banner-content h1 {
        font-size: 2.5rem;
    }
    .hero-banner {
        padding-top: 150px;
    }
}
