# Tree
# 이진 트리(binary tree)
모든 노드들의 자식 노드가 두 개 이하인 트리를 의미하는데, 다음은 이진 트리의 예다. 이런 이진 트리에서는 서브 트리가 두 개 이하기 떄문에 서브 트리는 왼쪽 서브 트리와 오른쪽 서브 트리로 구분한다.

![image](https://user-images.githubusercontent.com/126844596/227129551-8d022eb3-8105-45d4-988a-17fc2f3f1dd3.png)

# 완전 이진 트리(complete binary tree)
단말 노드를 제외한 나머지 두 개의 자식 노드를 가지고 있는 트리.

☆ 정이진 트리(full binary tree)는 양쪽이 대칭을 이루는 트리이다

![image](https://user-images.githubusercontent.com/126844596/227129940-9ca55e50-d372-4cd5-ac52-9288755735e5.png)

# 트리 전체 노드의 수 구하기
근 노드(root Node) 가 레벨1 인데 아래로 한칸씩 내려갈 때 마다 레벨1 씩 증가 한다.

전체 노드의 수 구하는 공식 : ![image](https://user-images.githubusercontent.com/126844596/227131335-870f8642-035c-4110-a105-b5907f44f960.png)

현재 레벨n에서의 노드수 구하는 공식 : ![image](https://user-images.githubusercontent.com/126844596/227132864-fecd2373-76ee-4cfc-b2c8-b9c987536f7d.png)

n은 레벨

● 전이진 트리(Complete Binary Tree)

전이진 트리는 노드의 수가n개일 때, 정이진 트리의 각 노드에 붙힌1~n의 일련번호와 1:1 대응되는 트리를 말한다.

※ 중간에 빈 부분이 있으면 전이진 트리가 될 수 없다.

![image](https://user-images.githubusercontent.com/126844596/227134706-bc702a03-5192-412e-9ad4-afe2153a47cc.png)

● 사향 이진 트리(Skewed Binary Tree)
사향 이진 트리는 루트 노드로 부터 왼쪽 또는 오른쪽으로만 기울어진 트리, 즉 왼쪽 또는 오른쪽 자식이 없는 노드들로 만 구성된 트리다.

-왼쪽 사향 이진 트리: 오른쪽 자식이 없는 노드들로 만 구성된 트리

-오른쪽 사향 이진 트리: 왼쪽 자식이 없는 노드들로 만 구성된 트리

![image](https://user-images.githubusercontent.com/126844596/227135687-3947f9d2-096b-42d1-be8a-9ee64ccf66f0.png)

● 이진 트리(binary tree)의 표현

이진트리는 배열이나 연결 리스트를 이용해서 구현할 수 있다

![image](https://user-images.githubusercontent.com/126844596/227391607-c2b0f2a1-80f2-4ed7-9bab-9843b07e2d7d.png)

● 이진 트리를 연결리스트로 표현한 예

![image](https://user-images.githubusercontent.com/126844596/227391713-2e3b29b0-7fbd-4364-a948-51dfb5d9b899.png)

● 이진 트리(binary tree)의 순희

이진 트리의 모든 노드를 특정한 순서대로 한 번씩 방문하는 것이다.

순회하는 방법에는 전위(preorder), 중위(inorder), 후위(postorder) 순회가 있다.

- 전위 순회(preorder)

노드(루트)를 먼저 방문하고 왼쪽 서브 트리, 오른쪽 서브 트리 순으로 방문 (Root->Left->Right)

![image](https://user-images.githubusercontent.com/126844596/227392729-0299e337-00d3-4790-88a3-fd7ae375e397.png)

- 중위 순회

왼쪽 서브 트리, 루트, 오른쪽 서브 트리 순으로 방문(Left->Root->Right)

![image](https://user-images.githubusercontent.com/126844596/227392784-96fabf28-e66e-4bc9-b052-2d3c2cc94fad.png)

- 후위 순회

왼쪽 서브 트리, 오른쪽 서브트리, 루트 순으로 방문(Left->Right->Root)

![image](https://user-images.githubusercontent.com/126844596/227393070-ad67bc24-0868-41b0-8a10-718a6c94b5ca.png)

● 이진 트리 탐색(Binary Search Tree)
이진 탐색 트리는 데이터 삽입, 삭제, 탐색 등이 자주 발생하는 경우에 효율적인 구조로, 이진 트리이면서 같은 값을 갖는 노드가 없어야 한다.

왼쪽 서브트리에 있는 모든 데이터는 현재 노드의 값보다 작고, 오른쪽 서브 트리에 있는 모든 노드의 데이터는 현재 노드의 값보다 크다.

● 데이터 탐색은 루트에서부터 시작된다.

-루트 노드의 데이터와 찾으려는 데이터를 비교하여 같으면 탐색은 성공 종료

-루트 노드가 작으면 루트 노드의 오른쪽

-루트 노드가 크면 루트 노드의 왼쪽

● 데이터가 8인 노드를 탐색하는 과정을 살펴보면

![image](https://user-images.githubusercontent.com/126844596/227395231-5b1fd49b-dcb6-4073-9884-3d7b0e516d07.png)

7-> 11-> 8

● 이진 트리 삽입

이진 탐색 트리에서의 삽입은 탐색 동작을 통해 이루어진다.
탐색에 성공하면 삽입은 실패하는데, 이는 이진 탐색 트리는 같은 데이터를 갖는 노드가 없어야 하기 때문이다.

반면에 탐색에 실패하면 삽입을 할 수 있으며, 탐색에 종료된 지점의 데이터를 값으로 하는 노드가 삽입된다.

삽입할 위치는 루트 노드에서부터 시작되며 삽입할 노드의 데이터가 비교하는 노드의 데이터보다 작으면 왼쪽 서브 트리로 진행하고 크면 오른쪽 서브 트리로 진행한다

![image](https://user-images.githubusercontent.com/126844596/227396220-111c82ec-820c-4912-be85-fefdfab1b249.png)

● 아잔 트리 삭제

이진 탐색 트리에서 노드를 삭제하는 동작은 삭제할 노드의 위치에 따라 세 가지로 구분된다.

● 삭제할 노드가 단말 노드인 경우

부모 노드에서 삭제할 노드를 가리키는 링크를 제거하면 된다

![image](https://user-images.githubusercontent.com/126844596/227396659-bdec73b8-eff0-4684-86a2-06c165de7cf2.png)

● 삭제할 노드의 자식 노드가 하나인 경우

부모 노드의서 삭제할 노드를 가리키는 링크를 삭제할 노드의 자식 노드를 가리킨다

![image](https://user-images.githubusercontent.com/126844596/227396792-55c04a83-5395-44e3-b731-41dc4111e520.png)

● 삭제할 노드의 자식 노드가 두 개인 경우

삭제할 노드를 왼쪽 서브트리에서 가장 큰 노드 또는 오른쪽 서브 트리에서 가장 작은 노드로 대체한다. 그리고 대체된 원래 노드를 삭제한다.

![image](https://user-images.githubusercontent.com/126844596/227397196-d564eaac-0af2-4cd4-9f55-e6c738c9d0cb.png)
