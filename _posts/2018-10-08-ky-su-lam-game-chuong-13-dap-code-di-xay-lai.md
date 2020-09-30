---
title: "[Ký sự làm game] Chương 13: Đập code đi xây lại"
date: "2018-10-08"
---

Mấy bài vừa rồi xàm lông hơi mạnh, giờ sê ri lại quay lại vụ làm gêm nhé. Giữa năm 2016, sau khi học xong năm thứ 4 và bước vào năm thứ 5 ở trường Bách Khoa, mình gia nhập một studio có tên là Tofu Games. Tại đây mình được tham gia vào một dự án sản xuất thực sự, không chỉ là làm những bản chơi thử (prototype) như lúc làm thực tập ở Hiker. Với một thằng chưa từng hoàn thành một dự án thương mại nào, mình rất hứng thú với công việc mới này cùng những thử thách mà nó mang lại.

Mình biết đến Tofu lúc mình nghỉ thực tập ở Hiker, anh Huy giám đốc có nói chuyện riêng với mình và thằng bạn làm thực tập cùng về dự định tương lai của hai đứa. Mình bày tỏ nguyện vọng vẫn muốn tiếp tục làm game, và được anh Huy giới thiệu cho vài cái tên, Tofu là một trong số đó. Sau vụ này mình mới biết là ngành game vốn nhỏ, nhiều anh em làm game lại rất khoái khi gặp người khác làm chung ngành, thành ra quen nhau rất nhiều. (Điều này có nghĩa là anh em mà có ý định phá phách gì thì cũng tém tém lại nhé, kẻo tiếng xấu đồn xa lại không có nơi nào nhận đâu)

Lần ấy đi phỏng vấn cũng ngộ. Lần đầu tiên có người hỏi mình là em thích phỏng vấn ở quán trà đá bình dân hay cà phê sang chảnh. Mình lúc ấy sinh viên, đi phỏng vấn mà trong túi có đúng 20k, nên chỉ dám bảo xuống trà đá. Nếu chẳng may cuối buổi tính sĩ diện nổi lên vẫn có thể vung tay gáy "anh để đó em trả cho" được. Cơ mà chắc chẳng ai để thằng sinh viên bao, nên mình về nhà mà tờ 20k vẫn nguyên vẹn. ![](assets/image/sexy_girl-e1507297936806.png)

Vậy là mình gia nhập Tofu với tư cách là nhân viên part-time, một buổi đi học, một buổi đi làm. Dự án mình làm với Tofu cũng là đồ án tốt nghiệp của mình luôn, điều này giúp mình có thể tập trung tối đa. Hồi ấy Tofu chia làm hai đội, một đội làm web game và đội kia thì làm game 3D với Unity. Mình được nhận vào để làm game 3D (mà thực ra bảo làm web game mình cũng éo biết làm). Đội hình thời điểm đấy đại khái như này (về sau có vài biến đổi, nhưng những người có mặt từ ngày đầu vẫn ở đó cho đến ngày mình nghỉ Tofu):

- Một art director, kiêm luôn nhiệm vụ UI artist với lead team. Nhân vật này chúng ta gọi là sếp 1.
- Một concept artist.
- Một UI artist nữa.
- Hai 3D artist.
- Một anim.
- Một game designer.
- Và hai code, tính cả thằng mới gia nhập là mình. Người còn lại ở Tofu đã lâu, tuổi tác cũng lớn, mình sẽ gọi là anh Cả.

Thực tế thì Galaxy Gunner, game mà mình làm ở Tofu, không phải là một game thành công về mặt thương mại hay tiếng tăm, cũng không phải là game có những thứ quá cao siêu về mặt kỹ thuật, nhưng nó là game thương mại đầu tiên mình tham gia sản xuất. Quá trình này không dài, nhưng mình nếm đủ cả vui và buồn với nó, thành ra với mình con game bình thường này có khá nhiều thứ đáng nhớ. Mình cũng cho rằng mình đã làm hết sức mình với nó, chỉ có điều một thời gian sau nhìn lại, khi mình đã cứng cáp hơn, thì mới thấy bản thân lúc ấy có nhiều hạn chế.

Công việc đầu tiên mình làm khi gia nhập, đó là làm quen với đám code hiện tại. Rối rắm kinh khủng. Có những file mà mình hay gọi là file "code thần" - một mình nó xử lý vài chục thứ xảy ra bên dưới một con game. Mà mấy thứ này lại đéo liên quan đến nhau mới nhục. Tên biến tên hàm thì đặt lung tung không theo một quy chuẩn nào cả, đọc đau hết cả mắt. Đôi khi lại lẫn vào một vài từ tiếng Kinh như _stopMoveLinhTinh_. Logic thì rối rắm, 7-8 lệnh if lồng vào nhau. Mà thôi, kể xấu về đám code ngày ấy thì có mà hết mẹ nó ngày, anh em chỉ cần biết là sau ngày đầu tiên gia nhập, mình đến gặp anh Cả bảo anh là phát triển tính năng mới với đám code này là không ổn, không khả thi. Và hai anh em gật gù với nhau là... thôi, đập đi xây lại. Đằng nào thời điểm đó mấy anh chị chịu trách nhiệm phần art cũng đang cong mông làm lại do đổi art style. ![](assets/image/sweat-e1507297981554.png)

![](assets/image/legacy.png)

_Pro tip #1: Khi phải làm quen với code của một project do người khác viết, đừng tin bản thân bạn. Hãy tin call stack._

![](https://neatrick.files.wordpress.com/2016/06/641372181.jpg?w=660)

_Pro tip #2: Đập đi viết lại một hai chỗ là chuyện thường ở huyện. Nhưng khi đập đi viết lại cả project như trường hợp trên thì không lành tí nào._

_Pro tip #3: Có thể hầu hết bạn không tin, nhưng hầu hết code trong dự án sản xuất đều như mứt cả._

![](assets/image/11m1fl.jpg)

Vậy là mấy hôm sau, mình ngồi nghiên cứu tài liệu của dự án một lượt. Vạch ra xem có những mảng lớn gì cần làm, rồi chọn một mảng để làm đầu tiên.  Hồi làm thực tập ở Hiker, anh Huy quy định mỗi ý tưởng chỉ phục vụ trong 3 tuần. 3 tuần trôi nhanh lắm, thành ra phải nghĩ thật kỹ xem cái gì làm trước cái gì làm sau. Kết hợp kinh nghiệm có sẵn này với việc trao đổi thường xuyên với game designer, cả đội tìm ra phương án triển khai khá nhanh. Anh Cả rất thoải mái, cho phép mình tuỳ nghi tác chiến, có gì khó thì hỏi anh. Mới mấy ngày đầu đã được ông anh tín nhiệm, mừng rớt nước mắt, tự nhủ bản thân phải vặn hết ga, triển hết võ để không phụ niềm tin của anh. ![](assets/image/beauty-e1507298864302.png)

Nhân nói về anh Cả. Anh Cả người tầm thước, tay chân chắc nịch, bụng hơi to, chắc vì uống bia nhiều, mà thực ra anh uống bia vl thật. Mình bây giờ chịu sự ảnh hưởng khá lớn từ anh Cả, sự ảnh hưởng này đến từ nhiều phía. Thực sự mà nói thì anh Cả khá bừa bộn, điều này có thể thấy rõ trong code và git commit message của anh. Mình khá ngăn nắp và khó tính, thành ra tiếp xúc với những thứ này làm mình hiểu rõ hơn cái gì là cái mình cần tránh. Hồi mới vào Tofu lúc nào mình cũng ra cằn nhằn với anh về vụ này - "code của anh xấu vkl, em xoá đi viết lại đây" - anh chỉ cười hề hề "chú thấy chỗ nào xoá được thì cứ xoá". Tuy nhiên, đằng sau những dòng code bừa bộn, những commit message qua loa là một ông anh rất nhiệt tình, đối đãi với mình như em anh vậy. Cái gì khó hỏi anh, anh giải thích cho cặn kẽ. Những lúc mình bật mode hung hãn, đòi làm những thứ hoang đường, anh cũng là người kìm mình lại bằng những câu chuyện kinh nghiệm cá nhân.

Mình làm việc trong dự án này khoảng 9 hay 10 tháng gì đó, trong quá trình này mình gặp khá nhiều người thú vị, trong đó có bác Hồ, người cho em tất cả... à không phải, người dạy mình code cặp.

Kỳ sau sẽ nói về nhân vật này.
