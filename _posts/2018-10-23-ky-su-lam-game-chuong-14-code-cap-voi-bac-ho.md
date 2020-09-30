---
title: "[Ký sự làm game] Chương 14: Code cặp với bác Hồ"
date: "2018-10-23"
---

Lúc đập code đi viết lại, mình máu lắm, quyết tâm tổ chức lại hệ thống sao cho chuẩn chỉ đẹp đẽ, dễ hiểu. Mình dành nhiều thời gian để vạch ra kế hoạch: chia con game thành các hệ thống gì và chức năng của từng hệ thống ra sao, rồi mỗi hệ thống được dựng lên bởi những thành phần gì. Sau vài buổi thực hiện việc này, mình xoa tay khoan khoái, mở Visual Studio lên và bắt đầu code theo những gì đã định từ trước. Với mỗi file code, mình cũng trau chuốt từng li từng tí một, đảm bảo mọi thứ đều rõ ràng, dễ hiểu. Code xong một file mình sẽ duyệt lại một lượt, thứ nhất là để chắc chắn rằng file đó tuân thủ những yêu cầu mình đặt ra, và thứ hai là để thủ dâm tinh thần - ai code mà đẹp, mà tinh tế thế chứ lị. ![](https://tongtunggiang.com/vi/assets/images/beauty-e1507298864302.png)

![](https://tongtunggiang.com/vi/assets/images/so_good.png)

Không còn những vòng lặp và biểu thức điều kiện thụt đầu dòng tận hai chục lần. Không còn những hàm dài 300 dòng. Không còn những file code thần 5000 dòng. Không còn những tên biến tên hàm đặt lung tung vô tổ chức. File code được căn chỉnh tử tế, đẹp đẽ. Code của mình đẹp, mọi chuyện đều tốt đẹp.

Cho đến một ngày, mình nhận ra là code của mình không đẹp như thế. Nó có tốt hơn và rõ ràng hơn so với đám code cũ, nhưng nó vẫn... không tốt. Không tốt tức là nó vẫn còn nhiều điểm chưa được, cần phải cải thiện. Người giúp mình nhận ra điều đó, chính là bác Hồ.

Bác Hồ gia nhập trong một ngày tháng 10, trong tiết trời thu dịu mát đặc trưng của Hà Nội. Trước đó mình chỉ nghe sếp 1 nói loáng thoáng là sắp có thêm code mới, đến ngày hôm nay mới được biết. Bác Hồ người thấp, ăn mặc chỉn chu, áo luôn bỏ trong quần. Ăn nói thì nhẹ nhàng từ tốn, khác hẳn mình với anh Cả. Bonus thêm nụ cười hiền từ lúc nào cũng sẵn sàng. Bác lại không ăn thịt mấy, chỉ ăn rau, nên bữa trưa lúc nào cũng tươi cười gắp hết thịt từ suất của bác cho mình. Sau này khi bác đã nghỉ việc, mình quen thói đi xin thịt từ suất của anh Cả, anh đéo cho, mình lại chép miệng với anh "Anh em như cái cờ cờ, cuối cùng chả ai tốt với em như bác Hồ cả". ![](https://tongtunggiang.com/vi/assets/images/cry-e1507298016854.png)

Sau thời gian đầu làm quen, một ngày bác Hồ đến chỗ mình nói:

_"Anh thấy chú code phần này không ổn. Chú nhồi nhiều thứ vào một chỗ quá, thành ra rối rắm và khó hiểu. Mỗi file code chỉ nên làm một thứ thôi"_

Trong sự kinh hoàng, mình nhận ra là bác nói đúng. Lấy ví dụ nhé: mình viết đúng 1 class để điều khiển tất tần tật mọi thứ liên quan tới người chơi, từ việc quay đi quay lại như thế nào, cơ chế bắn ra sao, bị thương kiểu gì, vân vân. Trong khi thực tế thì cơ chế bắn và trạng thái máu của người chơi hoàn toàn không liên quan tới nhau - chúng lẽ ra nên được tách thành hai phần. Mình không tách, nên khi bác Hồ vào đọc sẽ thấy rất phức tạp. Nói cách khác, mình kiểm soát độ phức tạp của code chưa được tốt.

(Ngoài lề chút: "độ phức tạp" ở đây có nghĩa là khi đọc, người đọc phải để ý đủ thứ bên lề mới có thể hiểu được hoàn toàn đoạn code. Hoàn toàn không liên quan gì tới khái niệm "độ phức tạp" được dùng để phân tích thuật toán đâu nhé)

Vậy là ngay buổi chiều hôm đó, mình ngồi lại với bác Hồ để duyệt lại đám code mình viết một lượt nữa để chỉ ra chỗ nào ôm nhiều thứ quá cần phải tách ra. Nói thật là mình vật lộn rất nhiều trong buổi chiều hôm đó, bởi mình phải tư duy theo một cách khác hẳn. Kết thúc buổi chiều, mình và bác Hồ thống nhất được một danh sách những thứ cần làm, theo tư tưởng là những công việc độc lập sẽ phải được đặt vào những chỗ độc lập, không chung chạ gì hết. Rất may là khối lượng không quá lớn, nên thời gian xử lý đống này không mất quá nhiều thời gian. Nếu lúc đấy đập code đi viết lại lần nữa chắc mình xấu hổ xin nghỉ việc luôn mất.

Bởi cách tư duy  mới là hoàn toàn mới mẻ với mình, bác Hồ gợi ý trò code cặp. Trò này khá đơn giản, mình với bác Hồ bắt cặp với nhau, một người code một người soi. Hết một việc hoặc hết một khoảng thời gian thì thay người, ông đang soi nhảy vào code và ngược lại. Mình hơi chần chừ, nhưng cũng tò mò, nên cuối cùng lại tặc lưỡi tham gia.

![](https://tongtunggiang.com/vi/assets/images/kg3cgpznfql01.jpg)

Hoá ra trò này vui hơn mình tưởng. Ông ngồi soi không chỉ có ngồi nhìn và ngáp như mình nghĩ lúc đầu, trái lại ông ngồi soi có thể chỉ ra những thứ mà ông ngồi code không nhận ra, lại có thể suy nghĩ đến thiết kế của file code ảnh hưởng thế nào đến tổng thể một cách thoải mái. Vai trò được đổi liên tục, thành ra cũng không bị chán. Ông ngồi code thì vừa có thêm áp lực từ ông ngồi soi, thành ra viết code phải cẩn thận hơn nhiều - có ai thích bị chửi đâu? Cùng lúc ấy, ông ngồi code cũng thoải mái hơn vì có người khác đang soát cho mình. Quả là một công đôi việc.

Trò này không kéo dài lâu, bởi khoảng hai đến ba ngày sau, khi mình đã quen với cách tư duy mới, thì code cặp lại thành một thứ kéo chậm tiến độ xuống. Lúc này thì chia ra mỗi người code một mảng lại nhanh hơn, nhất là khi các task nhỏ đã được thiết kế để có thể phát triển độc lập với nhau. Dù vậy thì mình rất biết ơn thời gian code cặp ngắn ngủi này, bởi nó giúp mình rất nhiều thứ. Mình rèn được cách nhìn code dưới góc nhìn của một người khác, mình hiểu rõ hơn về công việc mình đang thực hiện, và mình học được rất nhiều thứ hay ho khi chứng kiến bác Hồ xử lý. Cho đến giờ, tức là hơn 2 năm sau quãng thời gian ấy, mình vẫn thường xuyên áp dụng trò này ở Hiker, dĩ nhiên là ở một quy mô nhỏ hơn nhiều, khi mình gặp một vài vấn đề liên quan đến phần việc của người khác, và thường chỉ kéo dài khoảng 5 đến 10 phút.

Nói vậy không có nghĩa là code của mình và bác Hồ viết ra trong thời điểm này là hoàn hảo, không có gì đáng chê trách. Cụ thể là gì, kỳ sau nhân vật nhà thơ sẽ giải đáp.
