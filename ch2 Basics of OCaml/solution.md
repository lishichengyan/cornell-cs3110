## Exercise: values [✭]
```
int = 42  
bytes = "CS3110"
```
## Exercise: operators [✭✭]
```
42 * 10;;  
3.14 /. 2.0;;  
4.2 ** 7.0;;
```
## Exercise: equality [✭] 
```
42 = 42;;
true
"hi" = "hi"
true
"hi" == "hi"
false
```
## Exercise: assert [✭]
```
()  
exception
assert (2110 <> 3110);;
```
## Exercise: if [✭]
```
if 2 > 1 then 42 else 7;;
```
## Exercise: double fun [✭]
```
let double x = x*2;;
assert (double 7 = 14);;
```
## Exercise: more fun [✭✭]
```
let cube x = x*x*x;;

let sign x = if x > 0 then 1 else if x = 0 then 0 else -1;;

let pi = acos(-1.);;
let area r = pi*.r*.r;;
```
## Exercise: RMS [✭✭]
```
let rms x y = sqrt(x*.x +. y*.y);;
```
## Exercise: date fun [✭✭✭]
```
let validDate d m = 
if m = "Jan" || m = "Mar" || m = "May" || m = "Jul" || m = "Aug" || m = "Oct" || m = "Dec" then
  if 1 <= d && d <= 31 then true else false
else if m = "Feb" then
  if 1 <= d && d <= 28 then true else false
else
  if 1 <= d && d <= 30 then true else false;; 
```
## Exercise: editor tutorial [✭✭✭]
I love vim, emacs sucks.
## Exercise: master an editor [✭✭✭✭✭, advanced]  
I love vim, emacs sucks.
## Exercise: fib [✭✭]
```
let rec fib n = 
         match n with
         | 1 -> 1
         | 2 -> 1
         | _ -> fib (n-1) + fib (n-2)
;;
```
## Exercise: fib fast [✭✭✭]
```
let rec h n pp p = 
        if n = 1 then p
        else h (n-1) p (pp+p)
;;

let fib_fast n =
        h n 0 1
;;

1001
```
## Exercise: poly types [✭✭✭]
```
val f : bool -> bool = <fun>
val g : 'a -> bool -> 'a = <fun>
val h : bool -> 'a -> 'a -> 'a = <fun>
val i : bool -> 'a -> 'b -> 'a = <fun>  
```
## Exercise: divide [✭✭]
```
let divide ~numerator:(arg1:float) ~denominator:(arg2:float) = arg1 /. arg2;;
```
## Exercise: associativity [✭✭]
```
let add x y = x + y;;

int 
fun
int
error
```
## Exercise: average [✭✭]
```
let (+/.) x y = (x+.y) /. 2.;;
```
## Exercise: hello world [✭]
```
hello world!                                                                    
- : unit = ()  

hello world!- : unit = ()  
```
## Exercise: print int list rec [✭✭]
```
let rec print_int_list = function
| [] -> ()
| h::t -> print_int h;print_int_list t;;
```
## Exercise: print int list iter [✭✭]
```
let print_int_list' lst = 
List.iter ((fun x -> print_int x)) lst;; 
```

