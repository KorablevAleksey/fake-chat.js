# Fake-chat.js 📫
![Example №1](https://rah-emil.ru/img/fake-chat.js.jpg "Example №1")
**Fake-chat.js** - это удобный эмулятор чата.

------------
### Инструкция
Ваш html:
```html
<div id="chat"></div>
```
Ваш JavaScript:
```javascript
let chatjs = fakechat({
	target: document.getElementById('chat'),
	messages: [
		['Hello my friend!✌', 1000],
		['Looking for a plugin that simulates chat?', 3000],
		['You found it! - <b>Fake-chat.js</b>', 5000],
	],
	visible: true,
	adding: 'beforeend'
});

chatjs.init();
```

------------
### Параметры
| Параметр  | Тип  | Значение  |
| :------------ | :------------ | :------------ |
| target  | Object  | DOM элемент, в котором публикуются сообщения.  |
| messages  | Array  | Массив сообщений, где 1 параметр - текст сообщения, а 2 параметр - время публикации сообщения.  |
| visible  | Boolean  | Если true, то сообщения начнут публиковаться только когда чат появится в области видимости. **По умолчанию false**. |
| adding  | String  | Порядок публикации сообщений. [Куда по отношению к elem вставлять строку. Всего четыре варианта...](https://learn.javascript.ru/multi-insert "Куда по отношению к elem вставлять строку. Всего четыре варианта...") |
