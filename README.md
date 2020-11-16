# **[ emoji decoder ] - proposal**

As the title describes it, this `App` will allow the user to translate any messages received as `emoji`s and will show it in plain english, for example:<br>
```
       👁 === I
       🐗 === bored
 👁 am 🐗 === I am bored
```
```
        🐳 === well
        👁 === I
        🙏 === hope
🐳 👁 🙏 so === well I hope so
```
```
         👁 === I
         🐝 === be
         🍁 === lieve
👁 🐝 🍁 you === I believe you
```
These examples below are just a few of the translation each emoji character will have.
By entering the emoji it will be able to translate directly to a word or part of a word which it will make it easier for the user to actually read any code emoji messages.<br>

## **App Logic**<br>
How the `app` will actually interact with the user.
There will be an array of objects with properties describing certain information of each `emoji`. It will have the certain descriptions as shown in the following example:

```javascript
const emojis = [
    {
        symbol: '👽',
        letter: 'a',
        name: 'alien',
        categories: [
            'face',
        ],
    },
    {
        symbol:'👶',
        letter: 'b',
        name: 'baby',
        categories: [
            'face',
        ],
    },
]
```
This properties will help the user search for the suitable translation of each emoji input it.<br>
The main property will by the `name` property, which will be the main one to be use to look up for the right match of the `symbol` and `name` of the `emoji` input.<br>

## **Stretch Goals**<br>

One of the very important and valuable features in an app its being able to look up all the categories that is needed to show the exact translation of each `emoji`.<br>
The user will be able to look up all the categories `emoji`s by entering in the search box and in the terminal will display the symbol and name in order to see the right wording as shown below:

```javascript
> node main.js search category face
👽 alien
👶 baby
.
.
.
[etc...]
```