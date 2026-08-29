![[Pasted image 20260807234727.png]]
what is the data structure?
![[Pasted image 20260807235022.png]]
the first method of it is a data structure named Stack.

> [!NOTE] Stack
> What is a stack?
> $$it's \ a\ last-in\ first-out \ structure $$
> ![[Pasted image 20260808151801.png]]


![[Pasted image 20260808151818.png]]

it's a depth-first method.
and Here's the example:
![[Pasted image 20260808152523.png]]




> [!NOTE] quene
> What is a quene?
> $$it's \ a \ first-in\ first-out\ structure$$
> ![[Pasted image 20260808152130.png]]




> [!NOTE] Heuristic Method
> What is a Heuristic method? It's the original adding Manhattan distance.![[Pasted image 20260808160455.png]]
> 
> Why is it works?
> ![[Pasted image 20260808161158.png]]
> but when we use Manhatton Method,it leads us to a closer choice when we meet the square of 12,wit.the square of 11.
> Ofcourse we will meet some situation that can't be selected by  Manhatton method,for example the square of 8.
![[Pasted image 20260808161544.png]]
To sum up ,the heuristic method is based on the oringinal situation of DFM(depth-first-method),and then the Manhatton.

![[Pasted image 20260808162826.png]]
also,the heuristic method also has its reserval.And its the source of part of the name——"Greedy",which is meant that it reaches the best locally,but maybe not best remotely.


> [!NOTE] A* method
> what is a A*method?
> ![[Pasted image 20260812191957.png]]
> ![[Pasted image 20260812192106.png]]

And After that,we are looking forward to generalize a special type of  algorithm between two components named Minimax

> [!info] Minimax
> The main idea of it is to turn the wins or losts into number counts:![[Pasted image 20260812193402.png]]
> the X player means the Max count player,
> and the O player means the Min count player
what do we need in the detailed situation:![[Pasted image 20260812193841.png]]
but after that,we need to check how can we exactly determine the process by correctly set the functions.We can take the tic-tac-toe game as an example. 
The players function:
![[Pasted image 20260812194348.png]]
and then the actions function:
![[Pasted image 20260812194521.png]]
but how can it choose the choice?Through the Result function:
![[Pasted image 20260812194636.png]]
The the last ,we need a terminal to assign the result:![[Pasted image 20260812194754.png]]
Thus,we have Utility:
![[Pasted image 20260812194850.png]]
![[Pasted image 20260812195641.png]]
totally,it begins with![[Pasted image 20260812200033.png]]
and wirh concretelizing,it may become![[Pasted image 20260812200426.png]]
The basic solution is![[Pasted image 20260812201138.png]]
![[Pasted image 20260812201238.png]]
![[Pasted image 20260812201253.png]]

And the MiniMax is called
Alpha-Beta Pruning:
Alpha-Beta means the best and the worst choice exist at the same time;The pruning means there is a deep big long deep search tree.
