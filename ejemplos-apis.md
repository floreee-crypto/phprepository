# 100 ejemplos con APIs

1. Obtener clima actual

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.weather.example.com/v1/current?city=Madrid';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.weather.example.com/v1/current?city=Madrid'
   ```

2. Pronóstico semanal

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.weather.example.com/v1/forecast?city=Barcelona&days=7';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.weather.example.com/v1/forecast?city=Barcelona&days=7'
   ```

3. Alertas meteorológicas

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.weather.example.com/v1/alerts?region=ES-MD';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.weather.example.com/v1/alerts?region=ES-MD'
   ```

4. Buscar películas

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.movies.example.com/v1/search?query=Inception';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.movies.example.com/v1/search?query=Inception'
   ```

5. Detalle de película

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.movies.example.com/v1/movies/tt1375666';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.movies.example.com/v1/movies/tt1375666'
   ```

6. Listar géneros de películas

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.movies.example.com/v1/genres';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.movies.example.com/v1/genres'
   ```

7. Últimas noticias

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.news.example.com/v1/top?country=es';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.news.example.com/v1/top?country=es'
   ```

8. Buscar noticias por tema

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.news.example.com/v1/search?q=tecnología';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.news.example.com/v1/search?q=tecnología'
   ```

9. Detalle de noticia

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.news.example.com/v1/articles/12345';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.news.example.com/v1/articles/12345'
   ```

10. Cotización de acciones

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.finance.example.com/v1/quotes?symbol=AAPL';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.finance.example.com/v1/quotes?symbol=AAPL'
   ```

11. Historial de acciones

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.finance.example.com/v1/history?symbol=TSLA&range=1y';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.finance.example.com/v1/history?symbol=TSLA&range=1y'
   ```

12. Tipo de cambio

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.finance.example.com/v1/forex?base=EUR&quote=USD';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.finance.example.com/v1/forex?base=EUR&quote=USD'
   ```

13. Crear usuario

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.users.example.com/v1/users';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.users.example.com/v1/users' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

14. Obtener usuario

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.users.example.com/v1/users/987';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.users.example.com/v1/users/987'
   ```

15. Actualizar usuario

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.users.example.com/v1/users/987';
   $method = 'PATCH';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X PATCH 'https://api.users.example.com/v1/users/987' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

16. Eliminar usuario

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.users.example.com/v1/users/987';
   $method = 'DELETE';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X DELETE 'https://api.users.example.com/v1/users/987'
   ```

17. Listar productos

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.store.example.com/v1/products';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.store.example.com/v1/products'
   ```

18. Buscar productos

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.store.example.com/v1/products?query=auriculares';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.store.example.com/v1/products?query=auriculares'
   ```

19. Detalle de producto

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.store.example.com/v1/products/sku-1234';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.store.example.com/v1/products/sku-1234'
   ```

20. Crear pedido

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.store.example.com/v1/orders';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.store.example.com/v1/orders' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

21. Estado de pedido

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.store.example.com/v1/orders/ord-5678';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.store.example.com/v1/orders/ord-5678'
   ```

22. Cancelar pedido

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.store.example.com/v1/orders/ord-5678/cancel';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.store.example.com/v1/orders/ord-5678/cancel' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

23. Listar repositorios

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.code.example.com/v1/repos?owner=acme';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.code.example.com/v1/repos?owner=acme'
   ```

24. Detalle de repositorio

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.code.example.com/v1/repos/acme/app';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.code.example.com/v1/repos/acme/app'
   ```

25. Crear issue

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.code.example.com/v1/repos/acme/app/issues';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.code.example.com/v1/repos/acme/app/issues' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

26. Listar issues

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.code.example.com/v1/repos/acme/app/issues?state=open';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.code.example.com/v1/repos/acme/app/issues?state=open'
   ```

27. Comentarios de issue

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.code.example.com/v1/issues/42/comments';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.code.example.com/v1/issues/42/comments'
   ```

28. Traducir texto

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.translate.example.com/v1/translate';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.translate.example.com/v1/translate' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

29. Detectar idioma

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.translate.example.com/v1/detect';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.translate.example.com/v1/detect' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

30. Obtener sinónimos

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.lexicon.example.com/v1/synonyms?word=rápido';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.lexicon.example.com/v1/synonyms?word=rápido'
   ```

31. Crear evento en calendario

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.calendar.example.com/v1/events';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.calendar.example.com/v1/events' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

32. Listar eventos

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.calendar.example.com/v1/events?from=2024-01-01&to=2024-01-31';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.calendar.example.com/v1/events?from=2024-01-01&to=2024-01-31'
   ```

33. Actualizar evento

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.calendar.example.com/v1/events/evt-111';
   $method = 'PATCH';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X PATCH 'https://api.calendar.example.com/v1/events/evt-111' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

34. Eliminar evento

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.calendar.example.com/v1/events/evt-111';
   $method = 'DELETE';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X DELETE 'https://api.calendar.example.com/v1/events/evt-111'
   ```

35. Buscar vuelos

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.travel.example.com/v1/flights?from=MAD&to=BCN&date=2024-08-10';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.travel.example.com/v1/flights?from=MAD&to=BCN&date=2024-08-10'
   ```

36. Reservar vuelo

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.travel.example.com/v1/bookings';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.travel.example.com/v1/bookings' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

37. Listar hoteles

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.travel.example.com/v1/hotels?city=Sevilla';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.travel.example.com/v1/hotels?city=Sevilla'
   ```

38. Reservar hotel

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.travel.example.com/v1/hotel-bookings';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.travel.example.com/v1/hotel-bookings' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

39. Obtener ruta en mapa

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.maps.example.com/v1/route?from=40.4168,-3.7038&to=41.3874,2.1686';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.maps.example.com/v1/route?from=40.4168,-3.7038&to=41.3874,2.1686'
   ```

40. Buscar lugares

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.maps.example.com/v1/places?query=cafetería&near=Valencia';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.maps.example.com/v1/places?query=cafetería&near=Valencia'
   ```

41. Geocodificar dirección

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.maps.example.com/v1/geocode?address=Gran%20V%C3%ADa%2C%20Madrid';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.maps.example.com/v1/geocode?address=Gran%20V%C3%ADa%2C%20Madrid'
   ```

42. Revertir coordenadas

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.maps.example.com/v1/reverse?lat=40.4168&lng=-3.7038';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.maps.example.com/v1/reverse?lat=40.4168&lng=-3.7038'
   ```

43. Obtener catálogo de música

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.music.example.com/v1/albums?artist=Daft%20Punk';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.music.example.com/v1/albums?artist=Daft%20Punk'
   ```

44. Reproducir pista

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.music.example.com/v1/player/play';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.music.example.com/v1/player/play' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

45. Crear playlist

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.music.example.com/v1/playlists';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.music.example.com/v1/playlists' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

46. Añadir canción a playlist

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.music.example.com/v1/playlists/pl-99/tracks';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.music.example.com/v1/playlists/pl-99/tracks' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

47. Listar episodios de podcast

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.podcast.example.com/v1/shows/789/episodes';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.podcast.example.com/v1/shows/789/episodes'
   ```

48. Suscribirse a podcast

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.podcast.example.com/v1/subscriptions';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.podcast.example.com/v1/subscriptions' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

49. Obtener recetas

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.recipes.example.com/v1/search?ingredient=tomate';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.recipes.example.com/v1/search?ingredient=tomate'
   ```

50. Detalle de receta

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.recipes.example.com/v1/recipes/456';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.recipes.example.com/v1/recipes/456'
   ```

51. Crear receta

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.recipes.example.com/v1/recipes';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.recipes.example.com/v1/recipes' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

52. Calcular calorías

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.nutrition.example.com/v1/estimate';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.nutrition.example.com/v1/estimate' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

53. Registrar actividad física

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.fitness.example.com/v1/activities';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.fitness.example.com/v1/activities' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

54. Consultar pasos diarios

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.fitness.example.com/v1/steps?date=2024-05-01';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.fitness.example.com/v1/steps?date=2024-05-01'
   ```

55. Obtener libro

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.books.example.com/v1/books/isbn/9780140449136';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.books.example.com/v1/books/isbn/9780140449136'
   ```

56. Buscar libros

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.books.example.com/v1/search?q=Garc%C3%ADa%20M%C3%A1rquez';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.books.example.com/v1/search?q=Garc%C3%ADa%20M%C3%A1rquez'
   ```

57. Listar autores

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.books.example.com/v1/authors?country=ES';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.books.example.com/v1/authors?country=ES'
   ```

58. Crear lista de lectura

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.books.example.com/v1/reading-lists';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.books.example.com/v1/reading-lists' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

59. Consultar estado de paquete

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.shipping.example.com/v1/track/1Z999';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.shipping.example.com/v1/track/1Z999'
   ```

60. Crear envío

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.shipping.example.com/v1/shipments';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.shipping.example.com/v1/shipments' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

61. Obtener tasas de envío

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.shipping.example.com/v1/rates?from=ES&to=FR&weight=2';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.shipping.example.com/v1/rates?from=ES&to=FR&weight=2'
   ```

62. Validar dirección

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.address.example.com/v1/validate';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.address.example.com/v1/validate' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

63. Autenticar usuario

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.auth.example.com/v1/login';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.auth.example.com/v1/login' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

64. Renovar token

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.auth.example.com/v1/token/refresh';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.auth.example.com/v1/token/refresh' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

65. Cerrar sesión

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.auth.example.com/v1/logout';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.auth.example.com/v1/logout' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

66. Obtener catálogo de cursos

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.learn.example.com/v1/courses?category=programaci%C3%B3n';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.learn.example.com/v1/courses?category=programaci%C3%B3n'
   ```

67. Inscribirse a curso

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.learn.example.com/v1/enrollments';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.learn.example.com/v1/enrollments' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

68. Progreso del curso

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.learn.example.com/v1/enrollments/123/progress';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.learn.example.com/v1/enrollments/123/progress'
   ```

69. Enviar mensaje

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.chat.example.com/v1/messages';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.chat.example.com/v1/messages' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

70. Listar conversaciones

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.chat.example.com/v1/conversations';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.chat.example.com/v1/conversations'
   ```

71. Marcar mensaje como leído

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.chat.example.com/v1/messages/555/read';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.chat.example.com/v1/messages/555/read' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

72. Obtener plantilla de correo

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.email.example.com/v1/templates/welcome';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.email.example.com/v1/templates/welcome'
   ```

73. Enviar correo

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.email.example.com/v1/send';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.email.example.com/v1/send' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

74. Estadísticas de campaña

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.email.example.com/v1/campaigns/abc/stats';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.email.example.com/v1/campaigns/abc/stats'
   ```

75. Crear encuesta

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.surveys.example.com/v1/surveys';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.surveys.example.com/v1/surveys' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

76. Listar respuestas de encuesta

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.surveys.example.com/v1/surveys/321/responses';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.surveys.example.com/v1/surveys/321/responses'
   ```

77. Crear ticket de soporte

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.support.example.com/v1/tickets';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.support.example.com/v1/tickets' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

78. Estado de ticket

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.support.example.com/v1/tickets/t-1001';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.support.example.com/v1/tickets/t-1001'
   ```

79. Agregar comentario a ticket

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.support.example.com/v1/tickets/t-1001/comments';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.support.example.com/v1/tickets/t-1001/comments' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

80. Listar endpoints de estado

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.status.example.com/v1/services';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.status.example.com/v1/services'
   ```

81. Estado de servicio

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.status.example.com/v1/services/payments';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.status.example.com/v1/services/payments'
   ```

82. Registrar dispositivo IoT

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.iot.example.com/v1/devices';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.iot.example.com/v1/devices' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

83. Telemetría de dispositivo

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.iot.example.com/v1/devices/dev-77/telemetry';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.iot.example.com/v1/devices/dev-77/telemetry'
   ```

84. Enviar comando a dispositivo

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.iot.example.com/v1/devices/dev-77/commands';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.iot.example.com/v1/devices/dev-77/commands' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

85. Obtener lista de tareas

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.tasks.example.com/v1/tasks?assigned_to=me';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.tasks.example.com/v1/tasks?assigned_to=me'
   ```

86. Crear tarea

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.tasks.example.com/v1/tasks';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.tasks.example.com/v1/tasks' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

87. Actualizar tarea

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.tasks.example.com/v1/tasks/9001';
   $method = 'PATCH';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X PATCH 'https://api.tasks.example.com/v1/tasks/9001' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

88. Completar tarea

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.tasks.example.com/v1/tasks/9001/complete';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.tasks.example.com/v1/tasks/9001/complete' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

89. Listar imágenes en galería

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.photos.example.com/v1/albums/44/photos';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.photos.example.com/v1/albums/44/photos'
   ```

90. Subir imagen

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.photos.example.com/v1/photos';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.photos.example.com/v1/photos' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

91. Etiquetar imagen

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.photos.example.com/v1/photos/88/tags';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.photos.example.com/v1/photos/88/tags' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

92. Obtener métricas de sitio

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.analytics.example.com/v1/metrics?site=example.com&period=7d';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.analytics.example.com/v1/metrics?site=example.com&period=7d'
   ```

93. Listar eventos de analítica

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.analytics.example.com/v1/events?site=example.com';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.analytics.example.com/v1/events?site=example.com'
   ```

94. Crear webhooks

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.webhooks.example.com/v1/webhooks';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.webhooks.example.com/v1/webhooks' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

95. Listar webhooks

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.webhooks.example.com/v1/webhooks';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.webhooks.example.com/v1/webhooks'
   ```

96. Eliminar webhook

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.webhooks.example.com/v1/webhooks/wh-22';
   $method = 'DELETE';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X DELETE 'https://api.webhooks.example.com/v1/webhooks/wh-22'
   ```

97. Buscar usuarios en CRM

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.crm.example.com/v1/contacts?query=acme';
   $method = 'GET';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X GET 'https://api.crm.example.com/v1/contacts?query=acme'
   ```

98. Crear oportunidad en CRM

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.crm.example.com/v1/opportunities';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.crm.example.com/v1/opportunities' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

99. Actualizar contacto en CRM

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.crm.example.com/v1/contacts/321';
   $method = 'PATCH';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X PATCH 'https://api.crm.example.com/v1/contacts/321' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```

100. Exportar datos de CRM

   **PHP (cURL)**

   ```php
   <?php
   $url = 'https://api.crm.example.com/v1/exports';
   $method = 'POST';
   $ch = curl_init($url);
   curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
   curl_setopt($ch, CURLOPT_CUSTOMREQUEST, $method);
   $payload = json_encode(['example' => 'data']);
   curl_setopt($ch, CURLOPT_HTTPHEADER, ['Content-Type: application/json']);
   curl_setopt($ch, CURLOPT_POSTFIELDS, $payload);
   $response = curl_exec($ch);
   if ($response === false) {
       echo curl_error($ch);
   } else {
       echo $response;
   }
   curl_close($ch);
   ?>
   ```

   **cURL**

   ```bash
   curl -X POST 'https://api.crm.example.com/v1/exports' -H 'Content-Type: application/json' -d '{"example":"data"}'
   ```
