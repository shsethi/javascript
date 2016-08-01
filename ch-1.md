## bind and this

```javascript
var dog = {
  sound: "woof",
  speak: function(){
   console.log(this.sound);
  }
}
dog.speak();             //woof

var speakIt  = dog.speak;
speakIt();             //undefined

var speakItCorrect  = dog.speak.bind(dog);
speakItCorrect();  //woof


```

