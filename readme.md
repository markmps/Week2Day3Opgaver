Uge 36 opgaver - Mark Sørensen
projectet week3day3e7 indeholder exercise 7 og 8.

Besvarelsen for opgave 1-8:

1)
Vi fandt en keep-alive i vores http header
Keep-alive header holder forbindelsen oppe hele tiden.
2)
Jeg frå redirect og r.html. redirects header er keep-alive og det samme med r.html.
Det sker ved goGet metoden.
3)
Den starter ved http og redirecter dig https.
Den forstår du skriver http, men sender dig til https.
4a) code 500
java.lang.ArithmeticException: / by zero
	Ups.processRequest(Ups.java:34)
	Ups.doGet(Ups.java:62)
	javax.servlet.http.HttpServlet.service(HttpServlet.java:626)
	javax.servlet.http.HttpServlet.service(HttpServlet.java:733)
	org.apache.tomcat.websocket.server.WsFilter.doFilter(WsFilter.java:53)
Vi får 500 fordi der er fejl i koden og den ikke kan dividere med 0 som er en server error.

4b) code 404
Vi får 404 fordi prøver en path som vi ikke har oprettet en servlet til som er en client error.

6)
Getter viser det hele og post gemmer de ting du har hidden.

7)
f - Det er blevet med en metode som sætter et navn til en attribute som bliver gemt på sessionen. Hvis der ikke er lavet en navn, så laves der et.

8) Da cookies deler et flash plug-in så kan alle browsere se denne cookie. Vi har angivet at vores cookie skal have en leve tid på et år: cookie.setMaxAge(60 * 60 * 24 * 365);
Derfor uanset browser om vi lukker vores browsere eller skifter browser, så kan vi denne session som stadig er tilgængelig, fordi den er angivet til at varer et år. i princippet hvis vi slukkede vores pc
så vil sessionen stadig være der. Hvis vi åbner http header og kigger under response headers finder man følgende for mig: Set-Cookie: username=Mark; Max-Age=31536000; Expires=Thu, 02-Sep-2021 15:50:42 GMT
Så igen, den lever et års tid.
