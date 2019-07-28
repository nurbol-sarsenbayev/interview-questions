#### 1. What is wrong with this code?
```html
<div class="card">
    <a class="card__image" href="/car/1">
        <img src="./img/car.jpg" alt="" >
        <div class="card__hover">
            <a href="/car/1" class="button">Посмотреть</a>
        </div>
    </a>
    <h4 class="card__title">Машина</h4>
</div>
```
##### Answer:
Nested link elemets are not allowed.
