# Faux-Racket-Interpter

## This is a Faux-Racket-Interpreter using Monadic Binding 

Can be used to evaluate expressions and functions defintions.  <br/>

Here we assume that expressions have been tokenized.  <br/>

## Sample use 


data Ast = </br>
      Number Int </br>
    | Bin Op Ast Ast </br>
    | Fun String Ast </br>
    | With (String, Ast) Ast </br>
    | App Ast Ast </br>
    | Set String Ast </br>
    | Seq Ast Ast </br>
    | Var String </br>


interp :: Ast -> Env -> State Val </br>
interp (ADD 1 2) Empty --> Empty (Numb 3)  </br>


Feel free to use!! </br>
