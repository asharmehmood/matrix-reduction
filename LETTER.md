Hey Ash!

My name is David, I'm currently working on a web app which includes an algorithm running on the client. I've written a MVP which gives me a solution, but it's not the optimal solution and it's not nearly as optimized as it needs to be in order for me to release it. Since I'm working on other parts of the web app right now I thought I could use some help from you for this specific problem.

The project is written in TypeScript but if you're more comfortable with using plain JavaScript that's fine for me.

The problem consists of three steps, but the last step is the one that I need help to optimize. It is regarding merging together arrays into as few matrices as possible. I'll explain with example below:

The first step is to take a 2D matrix of integers and generate all of its possible combinations. If we for instance have matrix A = [[1, 2, 3], [1], [1, 2]], we get the combinations C = [[1, 1, 1], [1, 1, 2], [2, 1, 1], [2, 1, 2], [3, 1, 1], [3, 1, 2]]. This step is done in a efficient way already.

The second step is to filter (reduce) specific combinations based on some given condition. For instance, if either A[0] or A[2] has to be 1 one, we get the following combinations after filtering: C' = [[1, 1, 1], [1, 1, 2], [2, 1, 1], [3, 1, 1]]. This step is also done in a efficient way already.

The last step that I need your help with is merging the filtered combinations back into as few matrices as possible again. If we continue using the previous example C', an optimal solution would be: A' = [[[1], [1], [1, 2]], [[2, 3], [1], [1]]]. If we run the algorithm from step 1 on these two matrices and add all combinations together, it should output the same combinations as in step 2.

As I said before, my take on the last step is far too complex right now, but I'll include it anyway as an attachment alongside with a simple testing suite and the algorithms from step 1 and 2 + its helper functions. I've also included the instructions for installing + running the test suite in the README.md file, you will need to have Node and yarn (or npm) installed however.

If you need any more details please just send me a message and I'd explain it further!

Best regards,
David Söderberg



[1][1][1,2]
[2,3][1][1]
1,1,1
1,1,2
2,1,1
3,1,1
