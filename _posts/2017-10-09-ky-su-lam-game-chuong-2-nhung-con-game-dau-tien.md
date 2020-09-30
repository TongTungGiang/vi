---
title: "[Ký sự làm game] Chương 2: Những con game đầu tiên"
date: "2017-10-09"
---

Tiếp nối [chương 1](http://tongtunggiang.com/vi/2017/10/02/ky-su-lam-game-chuong-1-su-khoi-dau/), loạt bài ký sự làm game của mình lại trở lại với chương thứ 2 để kể về những gì đã đưa mình tới nghiệp làm game. Nếu xét toàn bộ quá trình mình bập vào lập trình, tức là lúc mình ngồi gõ lạch cạch với mấy con phím Mitsumi thần thánh với thằng Q trong phòng tin trường cấp 2, thì cơ hội đầu tiên cho mình mó vào một con game đó là vào năm lớp 11 tại cuộc thi Tin học trẻ không chuyên. Vì đã khá lâu rồi nên những gì mình nhớ về cuộc thi và con game rất mờ nhạt, nên mình sẽ không đi vào chi tiết. Mình sẽ tập trung kể về những con game mà mình làm hồi đi học Đại học, vì đây là những viên gạch đầu tiên cho sự nghiệp sau này của mình.

 

Con game đầu tiên trong đời đại học của mình là con game dành cho... Linux. Hồi ấy học kỳ hè, rảnh háng chẳng biết làm gì, thấy làm mấy ứng dụng đồng hồ báo thức với cả lên lịch nó cứ chán chán, mấy thằng lôi nhau ra làm game. Lọ mọ tìm sách vở kiếm được bộ mã nguồn game viết bằng C của thư viện Allegro (mình cá là hầu hết các bạn sẽ tự hỏi thư viện này là thư viện bỏ mẹ nào, nếu bạn làm thế thật thì đừng lo vì đến giờ mình cũng éo biết). Gọi là bộ mã nguồn cho khệnh, chứ toàn bộ "project" khi đó chỉ có một file .h và một file .cpp, cũng chẳng phức tạp hơn những gì được học là mấy. Game cũng đơn giản, chỉ có hai người chơi điều khiển hai cái xe tăng lao vào bắn nhau, thằng nào chết thằng đó thua. Chả có ảnh ọt gì sất, xe tăng gồm mấy hình vuông với chữ nhật màu khác nhau, vẽ hoàn toàn bằng code ![](assets/images/burn_joss_stick-e1507298028986.png).

\[caption id="" align="aligncenter" width="629"\]![](assets/images/kceku2f.png) Đây, hình thật cho dễ hình dung\[/caption\]

Sợ bị mang tiếng cọp pi mã nguồn, mấy thằng bắt đầu mổ xẻ, tìm cách viết mấy con xe tăng do máy điều khiển. Dù lúc thuyết trình cũng mạnh dạn bốc phét là game của chúng em có AI này nọ, thực ra chỉ có cho tăng đi thẳng, đâm phải tường thì tìm hướng khác, rẽ hoặc quay đầu, chấm hết ![](assets/images/sweat-e1507297981554.png).

Con game bắn xe tăng ở trên coi như màn khởi động, và mình bắt đầu thực sự nghiêm túc với hướng lập trình game từ môn Lập trình hướng đối tượng (OOP), diễn ra vào kỳ học sau đó. Lúc đó mình thấy (và đến giờ vẫn vậy) tư tưởng của lập trình hướng đối tượng rất hợp để làm game. Tiện nói, nếu bạn mới bắt đầu với lập trình game, mình khuyên bạn nên cố gắng nắm vững những nguyên tắc của lập trình hướng đối tượng. Về cơ bản, game cũng chỉ là những đối tượng như anh hùng, quái vật, xe tăng... tương tác với nhau bằng cách này hoặc cách khác mà thôi.

\[caption id="" align="aligncenter" width="960"\]![](https://camo.githubusercontent.com/1e8ead84dc975a16df7f80c803b231aba55109d1/68747470733a2f2f692e696d6775722e636f6d2f324d69736a42412e6a7067) Sản phẩm mà mình tự hào nhất suốt thời đại học\[/caption\]

Sản phẩm của môn OOP này, cho đến bây giờ, vẫn là một trong những sản phẩm mà mình thấy tự hào nhất, vì nó được hoàn thành một cách bài bản nhất. Những sản phẩm còn lại trong thời đại học của mình, ngoại trừ đồ án tốt nghiệp, không một cái nào đạt đến mức làm mình hài lòng như sản phẩm của môn OOP, cả về độ hoàn thiện của sản phẩm cũng như những chi tiết kỹ thuật mà nhóm mình đã thực hiện.

Hồi ấy nhóm mình có làm một cái framework, thực chất chỉ làm công việc gói các lời gọi của thư viện SDL lại thành những lệnh đơn giản và dùng được ngay cho những mục đích thông dụng như xử lý cửa sổ, hình ảnh, âm thanh hay font chữ. Ban đầu thực ra cũng không định làm framework đâu, cơ mà khi đổi từ OpenGL sang SDL thấy thốn quá, nên chắc cốp làm thêm một tầng ở giữa, sợ mấy hôm nữa lại đổi tiếp thì vỡ mồm. Của đáng tội, sản phẩm hồi đó cũng khệnh ![](assets/images/matrix-e1507559558105.png), có độ chục map làm sẵn gì đó, lại có cả tool vẽ map cho người chơi tự vẽ lấy mà chơi. Gameplay thì cũng đơn giản, nhưng vì framework sơ sài quá nên cứ vừa làm vừa đắp thêm vào, thành ra cũng chẳng nhanh.

Tiện kể về con game đó, hồi ấy mình có một suy nghĩ kiểu "kéo thả cùi vãi, code chay như tao mới khệnh". Đó là lý do mà thời điểm đó mình nhất quyết phản đối việc nhóm dùng các game engine như Unity chẳng hạn, vì mình cho rằng phải code chay mới là hiểu sâu, là hiểu bản chất, là "thượng đẳng", còn dùng engine, kéo thả là kiểu nông cạn, là làm xong sản phẩm xong để đó mà không hiểu, là "hạ đẳng". Cho đến giờ, mình gặp không ít những bạn có suy nghĩ "nói không với engine, nói có với code chay" giống mình thời đó, với những mức độ cực đoan khác nhau. Phần lớn trong số này là sinh viên hoặc người mới bắt đầu tham gia ngành công nghiệp game.

Đó thực sự là một suy nghĩ sai lầm, ít nhất là với những gì mình đã trải nghiệm suốt 3 năm qua. Chương sau mình sẽ dành để nói kỹ hơn về tư tưởng này.
