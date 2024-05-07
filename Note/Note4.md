SASS

4.0

    CSS dosent have -nesting , extend ...etc
    Good for responsive design 
    mix-in :   SCSS  -> pre processer (web pack , vite) 
    have to add to our vite : npm add -D sass
    you have to build for deployment.
    use $variable name like this 



4.1

    nesting 
    let us write nested CSS

    You can nesting in side of the parent 
    &:hover {}


4.2 

    @extend

        %alert{
            margin:10px;
            padding:10px 20px;
            border-radius: 10px;
            border:1px dashed black;

            }

            .sucess {
            @extend %alert;
            background-color: green;
            }
     you can extend like this. 


4.3
   
   mix-in
        @mixin alert($alertColor){
        margin:10px;
        padding:10px 20px;
        border-radius: 10px;
        border:1px dashed black;
        background-color: $alertColor;

        }

        .sucess {
        @include alert(green)
}
'@mixin' 은 js의 function과 같은 코드 덩어리를 만들고 이 function(@mixin으로 만들어진 코드 덩어리)이 argument(인자)를 받을 수 있게 한다.
'@include'를 사용하여 argument(인자)를 보내고 function을 불러온다.


4.4

    Responsive design using mixin

    