# java-interviews

Spring
* В чем разница между аннотациями @RequestParam (1) и @PathVariable (2) в Spring web-приложении
@RequestParam - отвечает за зараметры url-пути
@PathVariable - представляет значение, являющееся частью url-пути

* Как извлечь параметры GET запроса? (localhost:8080?name=Elon&surname=Musk)

C помощью объект класса HttpServletRequest public get(HttpServletRequest request) {}
В HttpServletRequest содержаться ВСЕ сведения о поступившем http-запросе.
Если такого параметра нет, то возвращается null

С помощью public get(@RequestParam("name") String name) {}
Если такого параметра нет, то ошибка 400. Добавить required=false -> ошибки не будет

Database
* Транзакция - последовательность операций над БД, переводящих ее из одного непротиворечивого состояния в другое непротиворечивое состояние
