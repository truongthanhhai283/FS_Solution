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

https://themify.me/themify-icons