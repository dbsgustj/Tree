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

# 트리(Tree)2
● 전이진 트리(Complete Binary Tree)

전이진 트리는 노드의 수가n개일 때, 정이진 트리의 각 노드에 붙힌1~n의 일련번호와 1:1 대응되는 트리를 말한다.

※ 중간에 빈 부분이 있으면 전이진 트리가 될 수 없다.

![image](https://user-images.githubusercontent.com/126844596/227134706-bc702a03-5192-412e-9ad4-afe2153a47cc.png)

● 사향 이진 트리(Skewed Binary Tree)
사향 이진 트리는 루트 노드로 부터 왼쪽 또는 오른쪽으로만 기울어진 트리, 즉 왼쪽 또는 오른쪽 자식이 없는 노드들로 만 구성된 트리다.

-왼쪽 사향 이진 트리: 오른쪽 자식이 없는 노드들로 만 구성된 트리

-오른쪽 사향 이진 트리: 왼쪽 자식이 없는 노드들로 만 구성된 트리

![image](https://user-images.githubusercontent.com/126844596/227135687-3947f9d2-096b-42d1-be8a-9ee64ccf66f0.png)

