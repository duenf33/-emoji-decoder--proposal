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

## **How the `app` works**<br>
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