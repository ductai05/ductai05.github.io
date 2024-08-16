---
title: "Cây AVL"
date: 2024-08-16T22:21:00+07:00
draft: false
# github_link: "https://github.com/gurusabarish/hugo-profile"
author: "Duc Tai"
tags:
  - DSA
  - AVL
  - FIT@HCMUS
image: /images/blog/avl-tree/avl-tree.png 
description: "Cấu trúc dữ liệu: Cây AVL"
toc: 
---

<figure style="text-align: center; margin-bottom: 20px;">
  <img src="/images/blog/roadmap/nmlt.png" alt="Đồ án Nhập môn lập trình" style="max-width: 90%; height: auto;">
  <figcaption style="font-size: 14px; color: #555;">Đồ án game Caro, Nhập môn lập trình.</figcaption>
</figure>

## CTDL Cây

**Cấu trúc dữ liệu cây** biểu diễn các **nút (node)** được kết nối bởi các cạnh. Chúng ta sẽ tìm hiểu về **Cây nhị phân (Binary Tree)**, **Cây tìm kiếm nhị phân (Binary Search Tree)** và **Cây AVL** trong bài viết này.

**Cây nhị phân** là một cấu trúc dữ liệu đặc biệt được sử dụng cho mục đích lưu trữ dữ liệu. Một cây nhị phân có một điều kiện đặc biệt là mỗi nút có thể có **tối đa hai nút con**. Một cây nhị phân tận dụng lợi thế của hai kiểu cấu trúc dữ liệu: một mảng đã sắp thứ tự và một danh sách liên kết (Linked List), do đó việc tìm kiếm sẽ nhanh như trong mảng đã sắp thứ tự và các thao tác chèn và xóa cũng sẽ nhanh bằng trong Linked List.

### Khái niệm

Một số khái niệm quan trọng liên quan đến cây nhị phân: 

- **Đường**: là một dãy các nút cùng với các cạnh của một cây.
- **Nút gốc (Root)**: nút trên cùng của cây được gọi là nút gốc. Một cây sẽ chỉ có một nút gốc và một đường xuất phát từ nút gốc tới bất kỳ nút nào khác. Nút gốc là nút duy nhất không có bất kỳ nút cha nào.
- **Nút cha**: bất kỳ nút nào ngoại trừ nút gốc mà có một cạnh hướng lên một nút khác thì được gọi là nút cha.
- **Nút con**: nút ở dưới một nút đã cho được kết nối bởi cạnh dưới của nó được gọi là nút con của nút đó.
- **Nút lá**: nút mà không có bất kỳ nút con nào thì được gọi là nút lá.
- **Cây con**: cây con biểu diễn các con của một nút.
- **Truy cập**: kiểm tra giá trị của một nút khi điều khiển là đang trên một nút đó.
- **Duyệt**: duyệt qua các nút theo một thứ tự nào đó.
- **Bậc**: bậc của một nút biểu diễn số con của một nút. Nếu nút gốc có bậc là 0, thì nút con tiếp theo sẽ có bậc là 1, và nút cháu của nó sẽ có bậc là 2, …
- **Khóa (Key)**: biểu diễn một giá trị của một nút dựa trên những gì mà một thao tác tìm kiếm thực hiện trên nút.

{{< highlight cpp >}}

int main(){
  return 1;
}

{{< /highlight >}}