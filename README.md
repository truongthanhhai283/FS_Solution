# FS_Solution
This's a project trainning FS solution

Solution:
Xác định flex container/item
    - justify-content: 
        space-between; //cách xa đều 1 trái/ 1 phải, space-around: có khoảng cách 2 bên, 
        space-evenly: khoảng cách các item = nhau
    - Flex: 1/ > 1 -> Chiếm hết khoảng không gian theo chiều main axis(ngang)
    -  Flex chia khổi:
        flex 1,2,..: 
    - Flex: mặc định zoom nhỏ thì co width lại
    - flex-wrap: xuống dòng khi co dãn width
      flex-wrap:none/wrap-reverse(đảo ngược khi xuống dòng).
    - căn giữa chiều dọc + ngang-> margin: auto;
    -  align-self: flex-end; reverse trên <-> dưới
    - flex-direction: column/row - reverse: đảo trục
    - Flex: 1 -> Flex-growth/shrink/basis

Oder : Vị trí -> Oder : 1,2, ...

Animation:
    @keyframes name{
    from{
        ....
    }
    to{
        .....
    }
}

    call: animation: name case timeduration;


Fix UI bug:
    1. Navbar font-size
    2. Navbar social-icons
    3. Navbar bell-icons
    4. Notification arrow top offset + z-index + border-radius
    5. Navbar margin beetween avatar + name
    6. User menu separate
    7. Logo link
    8. Search selection offset - top

    9. Header-QR -> z-index
    10. User menu offset-top
    11. Seach history z-index
    12. Cart z-index
    13. Cart product name limit
    14. Category style
    15. product border-radius
https://themify.me/themify-icons


*** Nguyên tắc làm responsive
    .grid {
        .row {
            .column{

            }
            . n -column{

            }
        }

        . n - row{

        }
    }
	
***** Responsive
		- Responsive Web Design (RWD) là xu hướng mới theo đó quy trình thiết kế và phát triển web sẽ đáp ứng mọi thiết bị và môi trường của người dùng theo các tiêu chí kích thước và chiều của màn hình thiết bị
		- Tối ưu trải nghiệm người dùng:
		 + Hiển thị rõ ràng các thành phần
		 + Ẩn/Hiện các thành phần phù hợp theo kích thước màn hình
		 
		- How to:
			using css to hid/show elements
		
		- Tools
			Chrome developerment tools
			Viewport resizer chrome extension
			
		
		** Khái niệm Viewport
			Viewport là khu vực mà người dùng có thể dòm thấy nội dung của trang web. Có thể tạm dịch là KHUNG NHÌN.

		** Media query (@media)
			@media not|only mediatype and (mediafeauture and/or/not mediafeauture{
			
				.....Css code
			}
			
			Keyword: 
				NOT -> Loại trừ
				ONLY -> 
				AND
				OR
			mediatypes: Trường hợp responsive 
				Print -> 
				Screen
				Speech
				ALL
				
			mediafeauture
				MIN-WIDTH: Lớn hơn
				MAX-WIDTH  Lớn hơn
			
			Polyfill: giúp S/dụng được mediaquery
				
		