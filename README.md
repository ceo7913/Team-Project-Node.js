# 프로젝트명
Node-Project(team)
 
## 프로젝트 의도
Node.js , MySql활용능력개선

## 역할 및 주요 기능
- 게시판 페이지
  > 하위 페이지로 모두 이동가능
    > 제목, 작성자, 작성일자, 조회수 확인가능 
    > Pagination 구현
    
- 게시판 작성 페이지
  > 게시판 글 작성 가능
  > DB 저장 가능
  > DB 수정 가능
    
- 게시판 상세페이지
  > 이전글, 다음글 확인가능
  > 댓글 기능, 대댓글 기능
  
- 회원가입 페이지
  > refesh, access 토큰 발급 및 express 세션에 저장

## 사용한 스택
<h4>- FRONT</h4>
<span>
<img src="https://img.shields.io/badge/html5-61DAFB?style=for-the-badge&logo=html5&logoColor=black">
<img src="https://img.shields.io/badge/css3-764ABC?style=for-the-badge&logo=css3&logoColor=white">
<img src="https://img.shields.io/badge/javascript-000000?style=for-the-badge&logo=javascript&logoColor=white">

<h4>- BACK</h4>
<span>
<img src="https://img.shields.io/badge/socket.io-3178C6?style=for-the-badge&logo=socket.io&logoColor=white">
<img src="https://img.shields.io/badge/node.js-4479A1?style=for-the-badge&logo=node.js&logoColor=white">
<img src="https://img.shields.io/badge/Express-E0234E?style=for-the-badge&logo=Express&logoColor=white">
<img src="https://img.shields.io/badge/mysql-2D3748?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/sequelize-2D3748?style=for-the-badge&logo=sequelize&logoColor=white">
<img src="https://img.shields.io/badge/JSONWebTokens-2D3748?style=for-the-badge&logo=JSONWebTokens&logoColor=white">
</span>

<h4>- Collaboration Tool</h4>
<span>
<img src="https://img.shields.io/badge/github.io-181717?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/notion-000000?style=for-the-badge&logo=notion&logoColor=white">
</span>

# 페이지 (Front)
![image](https://user-images.githubusercontent.com/106497516/225777943-5634f328-77a5-4781-b7a0-e5fb8f6096d9.png)
![image](https://user-images.githubusercontent.com/106497516/225778157-a7983536-0ce8-4d56-9a5f-303e9c888aa5.png)

## 프로젝트 파일 구조

```
📦Team-Project-Node.js
 ┣ 📂.git
 ┃ ┣ 📂hooks
 ┃ ┃ ┣ 📜applypatch-msg.sample
 ┃ ┃ ┣ 📜commit-msg.sample
 ┃ ┃ ┣ 📜fsmonitor-watchman.sample
 ┃ ┃ ┣ 📜post-update.sample
 ┃ ┃ ┣ 📜pre-applypatch.sample
 ┃ ┃ ┣ 📜pre-commit.sample
 ┃ ┃ ┣ 📜pre-merge-commit.sample
 ┃ ┃ ┣ 📜pre-push.sample
 ┃ ┃ ┣ 📜pre-rebase.sample
 ┃ ┃ ┣ 📜pre-receive.sample
 ┃ ┃ ┣ 📜prepare-commit-msg.sample
 ┃ ┃ ┣ 📜push-to-checkout.sample
 ┃ ┃ ┗ 📜update.sample
 ┃ ┣ 📂info
 ┃ ┃ ┗ 📜exclude
 ┃ ┣ 📂logs
 ┃ ┃ ┣ 📂refs
 ┃ ┃ ┃ ┣ 📂heads
 ┃ ┃ ┃ ┃ ┗ 📜main
 ┃ ┃ ┃ ┗ 📂remotes
 ┃ ┃ ┃ ┃ ┗ 📂origin
 ┃ ┃ ┃ ┃ ┃ ┗ 📜HEAD
 ┃ ┃ ┗ 📜HEAD
 ┃ ┣ 📂objects
 ┃ ┃ ┣ 📂info
 ┃ ┃ ┗ 📂pack
 ┃ ┃ ┃ ┣ 📜pack-3e236ba5f1914cc2edc31f68c3886129b79277d6.idx
 ┃ ┃ ┃ ┗ 📜pack-3e236ba5f1914cc2edc31f68c3886129b79277d6.pack
 ┃ ┣ 📂refs
 ┃ ┃ ┣ 📂heads
 ┃ ┃ ┃ ┗ 📜main
 ┃ ┃ ┣ 📂remotes
 ┃ ┃ ┃ ┗ 📂origin
 ┃ ┃ ┃ ┃ ┗ 📜HEAD
 ┃ ┃ ┗ 📂tags
 ┃ ┣ 📜config
 ┃ ┣ 📜description
 ┃ ┣ 📜HEAD
 ┃ ┣ 📜index
 ┃ ┗ 📜packed-refs
 ┣ 📂.vscode
 ┃ ┗ 📜settings.json
 ┣ 📂config
 ┃ ┗ 📜config.js
 ┣ 📂controllers
 ┃ ┣ 📜admin_controller.js
 ┃ ┣ 📜find_id_controller.js
 ┃ ┣ 📜free_board_controller.js
 ┃ ┣ 📜game_skin_products_controller.js
 ┃ ┣ 📜game_skin_user_controller.js
 ┃ ┣ 📜game_skin_wish_controller.js
 ┃ ┣ 📜index_controller.js
 ┃ ┣ 📜point_history_controller.js
 ┃ ┣ 📜qna_board_controller.js
 ┃ ┣ 📜qna_reply_controller.js
 ┃ ┣ 📜tip_board_controller.js
 ┃ ┣ 📜tip_reply_controller.js
 ┃ ┗ 📜user_controller.js
 ┣ 📂middlewares
 ┃ ┗ 📜session_middleware.js
 ┣ 📂model
 ┃ ┣ 📜authority.js
 ┃ ┣ 📜chatting.js
 ┃ ┣ 📜condition_user.js
 ┃ ┣ 📜free_board.js
 ┃ ┣ 📜free_reply.js
 ┃ ┣ 📜game_skin_products.js
 ┃ ┣ 📜game_skin_user.js
 ┃ ┣ 📜game_skin_wish.js
 ┃ ┣ 📜inactive_user.js
 ┃ ┣ 📜index.js
 ┃ ┣ 📜point_history.js
 ┃ ┣ 📜point_total.js
 ┃ ┣ 📜point_type.js
 ┃ ┣ 📜qna_board.js
 ┃ ┣ 📜qna_reply.js
 ┃ ┣ 📜tip_board.js
 ┃ ┣ 📜tip_reply.js
 ┃ ┗ 📜users.js
 ┣ 📂modules
 ┃ ┗ 📜common.js
 ┣ 📂public
 ┃ ┣ 📂audio
 ┃ ┃ ┣ 📜baseBgm.mp3
 ┃ ┃ ┣ 📜changeImage.mp3
 ┃ ┃ ┣ 📜doorOpen.mp3
 ┃ ┃ ┣ 📜moveBgm.mp3
 ┃ ┃ ┣ 📜누군가 도망치고 숨을 헐떡인다 효과음.mp3
 ┃ ┃ ┣ 📜비명소리 (조금과함).mp3
 ┃ ┃ ┣ 📜시작을 알리는 효과음.mp3
 ┃ ┃ ┗ 📜으스스한 분위기 깜놀 효과음.mp3
 ┃ ┣ 📂css
 ┃ ┃ ┣ 📜board_inside.css
 ┃ ┃ ┣ 📜board_list.css
 ┃ ┃ ┣ 📜chat_ui.css
 ┃ ┃ ┣ 📜common.css
 ┃ ┃ ┣ 📜find_pw.css
 ┃ ┃ ┣ 📜floating-button.css
 ┃ ┃ ┣ 📜game_reset.css
 ┃ ┃ ┣ 📜game_ui.css
 ┃ ┃ ┣ 📜home.css
 ┃ ┃ ┣ 📜index.css
 ┃ ┃ ┣ 📜mypage.css
 ┃ ┃ ┣ 📜mypage_edit.css
 ┃ ┃ ┣ 📜shop.css
 ┃ ┃ ┣ 📜signup.css
 ┃ ┃ ┗ 📜writing.css
 ┃ ┣ 📂data
 ┃ ┃ ┣ 📜game_audio.js
 ┃ ┃ ┣ 📜game_collisions.js
 ┃ ┃ ┣ 📜game_portals.js
 ┃ ┃ ┗ 📜game_stuffs.js
 ┃ ┣ 📂game_json
 ┃ ┃ ┣ 📜game_stg1.json
 ┃ ┃ ┣ 📜game_testSave.json
 ┃ ┃ ┗ 📜game_untitled.json
 ┃ ┣ 📂img
 ┃ ┃ ┣ 📂game_image
 ┃ ┃ ┃ ┣ 📂background
 ┃ ┃ ┃ ┃ ┣ 📜backgroundAfterStg1.png
 ┃ ┃ ┃ ┃ ┣ 📜backGroundBeforeStg1.png
 ┃ ┃ ┃ ┃ ┣ 📜backGroundStg2.png
 ┃ ┃ ┃ ┃ ┣ 📜ded image.png
 ┃ ┃ ┃ ┃ ┣ 📜FG2.png
 ┃ ┃ ┃ ┃ ┣ 📜foreGroundAfterStg1.png
 ┃ ┃ ┃ ┃ ┣ 📜foreGroundBeforeStg1.png
 ┃ ┃ ┃ ┃ ┣ 📜foreGroundStg2.png
 ┃ ┃ ┃ ┃ ┗ 📜startPage.png
 ┃ ┃ ┃ ┣ 📂character
 ┃ ┃ ┃ ┃ ┣ 📂load
 ┃ ┃ ┃ ┃ ┃ ┗ 📜Dr Frankenstein Face.png
 ┃ ┃ ┃ ┃ ┣ 📜$Dr Frankenstien (resizing).png
 ┃ ┃ ┃ ┃ ┗ 📜README.md
 ┃ ┃ ┃ ┗ 📂playImage
 ┃ ┃ ┃ ┃ ┣ 📜awl_1.png
 ┃ ┃ ┃ ┃ ┣ 📜awl_2.png
 ┃ ┃ ┃ ┃ ┣ 📜awl_3.png
 ┃ ┃ ┃ ┃ ┣ 📜findIt.png
 ┃ ┃ ┃ ┃ ┣ 📜ghost_1.jpeg
 ┃ ┃ ┃ ┃ ┣ 📜ghost_2.jpeg
 ┃ ┃ ┃ ┃ ┗ 📜knife.png
 ┃ ┃ ┣ 📜22lim-logo.svg
 ┃ ┃ ┣ 📜character.png
 ┃ ┃ ┣ 📜coin.png
 ┃ ┃ ┣ 📜google-icon.svg
 ┃ ┃ ┣ 📜HC_Humans3A.png
 ┃ ┃ ┣ 📜HC_Humans3B.png
 ┃ ┃ ┣ 📜HC_Humans4A.png
 ┃ ┃ ┣ 📜HC_Humans4B.png
 ┃ ┃ ┣ 📜HC_Service_Dogs 2.png
 ┃ ┃ ┣ 📜HC_Service_Dogs.png
 ┃ ┃ ┣ 📜HC_Zombies3C.png
 ┃ ┃ ┣ 📜heart1.png
 ┃ ┃ ┣ 📜heart2.png
 ┃ ┃ ┗ 📜hospital-building.png
 ┃ ┗ 📂js
 ┃ ┃ ┣ 📂game_js
 ┃ ┃ ┃ ┣ 📂utill
 ┃ ┃ ┃ ┃ ┣ 📜game_func_inventory.js
 ┃ ┃ ┃ ┃ ┣ 📜game_func_stuff.js
 ┃ ┃ ┃ ┃ ┗ 📜game_func_ui.js
 ┃ ┃ ┃ ┣ 📜game_canvas_1.js
 ┃ ┃ ┃ ┣ 📜game_canvas_2.js
 ┃ ┃ ┃ ┣ 📜game_classes.js
 ┃ ┃ ┃ ┣ 📜game_common.js
 ┃ ┃ ┃ ┣ 📜game_playerclass.js
 ┃ ┃ ┃ ┗ 📜game_ui.js
 ┃ ┃ ┣ 📜borad_inside.js
 ┃ ┃ ┣ 📜borad_list.js
 ┃ ┃ ┣ 📜chat_ui.js
 ┃ ┃ ┣ 📜check_password.js
 ┃ ┃ ┣ 📜index.js
 ┃ ┃ ┣ 📜logo.js
 ┃ ┃ ┣ 📜shop.js
 ┃ ┃ ┣ 📜user_list.js
 ┃ ┃ ┣ 📜validity.js
 ┃ ┃ ┗ 📜writing.js
 ┣ 📂routers
 ┃ ┣ 📜admin_router.js
 ┃ ┣ 📜free_board_router.js
 ┃ ┣ 📜game_paranoia_router.js
 ┃ ┣ 📜game_skin_products_router.js
 ┃ ┣ 📜game_skin_user_router.js
 ┃ ┣ 📜game_skin_wish_router.js
 ┃ ┣ 📜index_router.js
 ┃ ┣ 📜qna_board_router.js
 ┃ ┣ 📜qna_reply_router.js
 ┃ ┣ 📜tip_board_router.js
 ┃ ┣ 📜tip_reply_router.js
 ┃ ┗ 📜user_router.js
 ┣ 📂service
 ┃ ┣ 📜encryption_service.js
 ┃ ┣ 📜free_board_service.js
 ┃ ┣ 📜game_skin_products_service.js
 ┃ ┣ 📜game_skin_user_service.js
 ┃ ┣ 📜game_skin_wish_service.js
 ┃ ┣ 📜inactive_user_service.js
 ┃ ┣ 📜index.js
 ┃ ┣ 📜point_history_service.js
 ┃ ┣ 📜point_total_service.js
 ┃ ┣ 📜qna_board_service.js
 ┃ ┣ 📜qna_reply_service.js
 ┃ ┣ 📜random.js
 ┃ ┣ 📜tip_board_sevice.js
 ┃ ┣ 📜tip_reply_sevice.js
 ┃ ┣ 📜token_service.js
 ┃ ┗ 📜user_service.js
 ┣ 📂view
 ┃ ┣ 📂partial
 ┃ ┃ ┣ 📜footer.html
 ┃ ┃ ┣ 📜header_down.html
 ┃ ┃ ┗ 📜header_up.html
 ┃ ┣ 📜admin_chatlist.html
 ┃ ┣ 📜board_inside.html
 ┃ ┣ 📜board_list.html
 ┃ ┣ 📜change_pw.html
 ┃ ┣ 📜ex.chat_ui.html
 ┃ ┣ 📜find_id.html
 ┃ ┣ 📜find_pw.html
 ┃ ┣ 📜floating-button.html
 ┃ ┣ 📜free_board_insert.html
 ┃ ┣ 📜free_board_list.html
 ┃ ┣ 📜free_board_update.html
 ┃ ┣ 📜free_board_view.html
 ┃ ┣ 📜game_paranoia.html
 ┃ ┣ 📜index.html
 ┃ ┣ 📜login.html
 ┃ ┣ 📜mypage.html
 ┃ ┣ 📜mypage_edit.html
 ┃ ┣ 📜point_history.html
 ┃ ┣ 📜qna_board_insert.html
 ┃ ┣ 📜qna_board_list.html
 ┃ ┣ 📜qna_board_update.html
 ┃ ┣ 📜qna_board_view.html
 ┃ ┣ 📜shop.html
 ┃ ┣ 📜signup.html
 ┃ ┣ 📜skin_list.html
 ┃ ┣ 📜tip_board_insert.html
 ┃ ┣ 📜tip_board_list.html
 ┃ ┣ 📜tip_board_update.html
 ┃ ┣ 📜tip_board_view.html
 ┃ ┣ 📜update_pw.html
 ┃ ┣ 📜user_list.html
 ┃ ┗ 📜writing.html
 ┣ 📜.gitignore
 ┣ 📜app.js
 ┣ 📜package-lock.json
 ┣ 📜package.json
 ┗ 📜README.md
```
       
