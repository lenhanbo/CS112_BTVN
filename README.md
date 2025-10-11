## Đề bài:
Bạn đang làm ở văn phòng quản lý nhân sự ở trong một công ty gồm $n$ người. 

Mỗi nhân viên sẽ có chính xác một người là quản lý của mình trừ nhân viên có chỉ số $1$. 

Người thứ $i$ sẽ có một khối lượng công việc $w_i$. 

Định nghĩa chỉ số phức tạp công việc của người thứ $i$ là $C_i = \sum_{j} (w_j + 1)$ trong đó $j$ là nhân viên mà $i$ quản lý.

Bạn được giao nhiệm vụ cắt giảm nhân sự. Bạn có thể chọn một vài người để sa thải khỏi công ty. 
- Tất cả nhân viên được quản lý bởi một người bị sa thải sẽ được tiếp nhận bởi quản lý của người đó. 
- Đồng thời, khối lượng công việc của người bị sa thải cũng sẽ được chuyển giao cho quản lý của người đó.
- Công ty sẽ không muốn nhân viên của mình phải chịu quá nhiều trách nhiệm nên trong mọi thời điểm, độ ~~pc~~ phức tạp công việc của mỗi nhân viên không được vượt quá mức pickle ball $m$.
- Hiển nhiên, nhân viên có chỉ số $1$ là CEO của công ty nên bạn không thể sa thải.
Hãy tìm số lượng người tối đa mà bạn có thể sai thải !!
## Input : 
- Dòng đầu gồm $2$ số nguyên $n$, $m$.
- Dòng tiếp theo gồm $n$ số nguyên $w_i$.
- $n-1$ dòng tiếp theo, dòng thứ $i$  gồm $1$ số nguyên $p_i$ là quản lý của nhân viên có chỉ số $i+1$.

## Output:
- Gồm một số nguyên là số lượng người tối đa mà bạn có thể sa thải.

## Giới hạn:
- Subtask 1(2 điểm) : $n \le 18$.
- Subtask 2(2 điểm) : $n \le 676767, m\le 369$.
- Subtask 3(6 điểm) : Không có ràng buộc.
- Trong mọi bộ test : $n \le 696969; m \le 36363636;0 \le c_i \le m;0\le w_i \le m$.

## Ví dụ:
### Input 
```
4 6 
0 6 2 3
1
1
3
```
### Output
```
2
```
Giải thích : Sa thải $2$ nhân viên có chỉ số $3$ và $4$. Có thể chứng minh không tồn tại cách sa thải khác tốt hơn.

