# Вопросы к собеседованию на позицию Java Developer

## **Spring**
1. В чем разница между аннотациями **@RequestParam** и @PathVariable в Spring web-приложении

- **@RequestParam** - отвечает за зараметры url-пути

- **@PathVariable** - представляет значение, являющееся частью url-пути

2. Как извлечь параметры GET запроса? (localhost:8080?name=Elon&surname=Musk)

- **HttpServletRequest**: C помощью объект класса HttpServletRequest public get(***HttpServletRequest request***) {}
  
  В **HttpServletRequest** содержатся ВСЕ сведения о поступившем http-запросе.
  
  Если такого параметра нет, то возвращается null.

- **@RequestParam**: С помощью public get(***@RequestParam("name") String name***) {}
  Если такого параметра нет, то ошибка 400. Добавить required=false -> ошибки не будет

## **Database**
* Транзакция - последовательность операций над БД, переводящих ее из одного непротиворечивого состояния в другое непротиворечивое состояние


## **Kafka**
1. Что такое topic?
2. Что такое partition?
3. Что такое zookeeper?
4. Как сделать так, чтобы сообщения, принадлежащие одной логической группе всегда попадали в одну патрицию?
5. Зачем нужно consumer group?
6. Гарантии доставки?
7. Что такое kafka streams?
8. Что такое auto.offset.reset?
