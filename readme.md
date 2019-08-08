# chrome issue

when I use chrome device toolbar, "input range" doesn't work.
like that


I think chrome default css of input range for device toolbar is broken
I guess that the css should like that.

![sample](./problem.html)


# fixed
![sample](./solved.html)



```css
        input[type=range] {
            -webkit-appearance: none;
            background: #5e5e5e;
            height: 100%;
            width: 100%;
        }
        input[type=range]::-webkit-slider-thumb {
            -webkit-appearance: none;
            background: #5e5e5e;
            height: 10px;
            width: 10px;
            border-radius: 50%;
        }
```