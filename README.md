
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Запуск JMeter тестов</title>
</head>
<body>

<h1>Запуск JMeter тестов</h1>

<h2>Запуск тестов в режиме Non-GUI</h2>

<p>Для запуска тестов JMeter в режиме Non-GUI через Maven выполните команду:</p>

<pre><code>mvn clean verify</code></pre>

<p>Тесты будут выполнены в фоновом режиме без графического интерфейса.</p>

<h2>Запуск тестов в режиме GUI</h2>

<p>Для запуска тестов JMeter в режиме GUI через Maven выполните следующие команды:</p>

<pre><code>mvn jmeter:configure jmeter:gui</code></pre>

<p>Эта команда откроет JMeter в графическом интерфейсе, позволяя вам взаимодействовать с вашими тестами в удобной среде.</p>

<h2>Запуск тестов JMeter с применением заготовленных профилей </h2>

<p>Для запуска тестов JMeter в режиме Non-GUI через Maven с применением заготовленных профилей необходимо приписать к команте запуска теста параметр -P <название теста> stab - тест со стабильной нагзукой </p>
<p>stab - тест со стабильной нагзукой</P>
<p>maxperf - тест с линейно нарастающей нагрузкой</P>
<pre><code>mvn clean verify -P stab 
mvn clean verify -P maxperf</code></pre>
</body>
</html>
