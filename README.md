<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Uy Tín Tạo Nên Thương Hiệu!" />
    <meta name="author" content="OTISStore" />
    <meta
      name="image"
      content="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png"
    />
    <title>OTISStore | Uy Tín Tạo Nên Thương Hiệu!</title>
    <link
      rel="icon"
      type="image/jpeg"
      href="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
    />

    <!-- Google Analytics -->
    <script
      async
      src="https://www.googletagmanager.com/gtag/js?id=G-H6LM2XKZTS"
    ></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag() {
        dataLayer.push(arguments);
      }
      gtag("js", new Date());
      gtag("config", "G-H6LM2XKZTS");
    </script>

    <style>
      html {
        overflow: -moz-scrollbars-none; /* Firefox cũ */
        scrollbar-width: none; /* Firefox mới */
        scroll-behavior: smooth; /* Cuộn mượt */
      }
      ::-webkit-scrollbar {
        width: 0 !important; /* 🎯 Không chiếm không gian */
        height: 0 !important;
        display: none !important; /* 🎯 Ẩn hoàn toàn */
      }
      /* 🎯 Đảm bảo không có padding/margin cho thanh cuộn */
      * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
      }

      body {
        font-family: "Segoe UI", sans-serif;
        background-color: #000000;
        color: #000000;
      }

      /* Header */
      .body-top {
        width: 100vw;
        height: 75px;
        background-color: #000000;
        position: fixed;
        top: 0;
        left: 0;
        display: flex; /* dùng flexbox để căn giữa nội dung */
        align-items: center;
        align-content: center;
        justify-content: center;
      }

      .body-top .img {
        width: min(100px, 10%);
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .body-top .img img {
        height: 60px;
        border-radius: 50%;
        margin: auto;
        box-shadow:
          0 0 10px rgb(226, 226, 226),
          0 0 10px rgb(250, 250, 250);
      }

      .menu {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;
        width: max(80%, 100% - 200px);
      }

      .menu label {
        width: max(120px, 30%);
        text-align: center;
        padding: 0px 5px;
      }

      .menu label a {
        width: 100%;
        font-size: clamp(15px, 1.8vw, 24px);
        font-family: "Montserrat", sans-serif;
        letter-spacing: 1px;
        text-align: center;
        padding: 0px 5px;
        color: #e4e0e0c7;
        font-weight: 600;
        text-decoration: none;
      }

      .menu label a:hover {
        color: rgba(123, 226, 255, 0.867);
      }

      @media (max-width: 600px) {
        .body-top .img {
          display: none;
        }

        .menu {
          width: 100%;
        }

        .menu label {
          width: 30%;
        }

        .menu label a {
          font-size: 15px;
        }
      }

      .body-bottom {
        position: absolute;
        top: 80px;
        left: 50%;
        transform: translateX(-50%); /* dịch tâm khối về chính giữa */

        width: 100vw;
        min-width: 400px;
        height: calc(100vh - 80px);
        overflow-x: scroll;

        font-family: "Segoe UI", sans-serif;
        background-color: #000000;
        color: #ffffff;
      }

      .header {
        width: 100vw;
        padding: 10px 20px 15px 20px;
        min-width: 400px;
        height: auto;
        display: flex;
        background-color: #000000;
        border-top: 2px solid #ffffff;
        align-items: center;
        align-content: center;
        justify-items: center;
        justify-content: center;
      }

      .header strong {
        font-size: clamp(14px, 1.8vw, 24px);
        color: #ffffff;
        height: 28px;
        text-shadow:
          0 0 2px rgba(255, 255, 255, 0.748),
          0 0 5px rgb(122, 177, 255);
      }

      .panel {
        width: 100vw;
        aspect-ratio: 1920/360;
        margin: 0 auto;
      }

      /* VIDEO REVIEW */
      .video-container {
        width: 100%;
        height: auto;
        min-width: 320px;
        max-height: calc(100dvh - 80px);
        aspect-ratio: 16 / 9;
        margin: 0 auto;
        border-radius: 5px;
        display: flex;
        background: #000000;
        align-items: center; /* Căn giữa theo chiều dọc */
        align-content: center;
        justify-content: center; /* Căn giữa theo chiều ngang */
        justify-items: center;
        position: relative;
        flex-direction: column; /* Nếu bạn có nhiều post, vẫn xếp theo dòng */
      }

      .video-content {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: stretch;
        width: 100vw;
        background: black;
        gap: 10px;
        padding: 10px;
      }

      .video-content .video-box {
        flex: 1 1 480px;
        max-width: 50%;
        aspect-ratio: 16/9;
        background-color: #000000;
      }

      .video-content .video-box iframe {
        width: 100%;
        height: 100%;
        border: none;
      }

      @media (max-width: 900px) {
        .video-content .video-box {
          flex: 1 1 420px;
        }
      }

      @media (max-width: 600px) {
        .video-content .video-box {
          flex: 1 1 360px;
          max-width: 100%;
        }
      }

      .group-content {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: stretch;
        width: 100vw;
        background: black;
        gap: 10px;
        padding: 10px;
      }

      .group-content .group-box {
        flex: 1 1 200px;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 5px;
        transition: all 0.5s ease;
        border-radius: 5px;
        border: white solid 1px;
        overflow: hidden;
      }

      .group-content .group-box:hover {
        box-shadow: 0 0 10px rgb(255, 255, 255);
        transform: translateY(-5px);
      }

      .group-content .group-box img {
        width: 100%;
        height: auto;
        aspect-ratio: 16/9;
        object-fit: cover;
        border-radius: 5px;
      }

      .group-content .group-box a {
        width: 100%;
        text-align: center;
        color: #000;
        font-size: 18px;
        margin-top: 5px;
        text-decoration: none;
        font-weight: bold;
        text-shadow: 0 0 5px rgba(255, 255, 255, 0.5);
        background: linear-gradient(
          90deg,
          red,
          yellow,
          lime,
          cyan,
          blue,
          magenta,
          red
        );

        background-size: 300% auto;
        background-clip: text;
        /* -webkit-background-clip: text; */
        -webkit-text-fill-color: transparent;
        animation: moveColor 5s linear infinite;
      }

      .group-content .group-box .a1 {
        background: linear-gradient(
          90deg,
          red,
          yellow,
          lime,
          cyan,
          blue,
          magenta,
          red
        );
      }

      @keyframes moveColor {
        from {
          background-position: 0% center;
        }
        to {
          background-position: 300% center;
        }
      }

      @media (max-width: 900px) {
        .group-content .group-box {
          flex: 1 1 calc(50% - 20px);
        }
      }

      @media (max-width: 600px) {
        .group-content .group-box {
          flex: 1 1 100%;
        }
      }

      .list-item,
      .list-acc {
        width: 100vw;
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        padding: 20px;
        justify-items: center;
        align-items: center;
        align-content: center;
        justify-content: center;
      }

      :root {
        --speed: 5s;
        --size: 3px;
      }

      .product-Items {
        width: clamp(120px, 30%, 210px);
        height: auto;
        min-height: 150px;
        background-color: #1c1c1c;
        border-radius: 5px;
        padding: 5px;
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        position: relative;
        overflow: hidden;
      }

      /* ===== CHUNG ===== */
      .product-Items span {
        position: absolute;
        display: block;
        filter: drop-shadow(0 0 6px var(--color));
        opacity: 0;
      }

      /* ===== TOP ===== */
      .product-Items .top {
        top: 0;
        left: -100%;
        width: 100%;
        height: var(--size);
        background: linear-gradient(
          90deg,
          transparent,
          var(--color),
          transparent
        );
      }

      /* ===== RIGHT ===== */
      .product-Items .right {
        top: -100%;
        right: 0;
        width: var(--size);
        height: 100%;
        background: linear-gradient(
          180deg,
          transparent,
          var(--color),
          transparent
        );
      }

      /* ===== BOTTOM (FIX CHUẨN) ===== */
      .product-Items .bottom {
        bottom: 0; /* ✅ đúng vị trí */
        top: auto; /* ❗ xoá ảnh hưởng top */

        right: -100%;
        left: auto;

        width: 100%;
        height: var(--size);

        background: linear-gradient(
          270deg,
          transparent,
          var(--color),
          transparent
        );
      }

      /* ===== LEFT ===== */
      .product-Items .left {
        bottom: -100%;
        left: 0;
        width: var(--size);
        height: 100%;
        background: linear-gradient(
          0deg,
          transparent,
          var(--color),
          transparent
        );
      }

      /* ===== HOVER ===== */
      .product-Items span {
        opacity: 1;
      }

      .product-Items .top {
        animation: runTop var(--speed) linear infinite;
      }

      .product-Items .right {
        animation: runRight var(--speed) linear infinite;
      }

      .product-Items .bottom {
        animation: runBottom var(--speed) linear infinite;
      }

      .product-Items .left {
        animation: runLeft var(--speed) linear infinite;
      }

      /* ===== KEYFRAMES ===== */
      @keyframes runTop {
        0% {
          left: -100%;
        }
        100% {
          left: 100%;
        }
      }

      @keyframes runRight {
        0% {
          top: -100%;
        }
        100% {
          top: 100%;
        }
      }

      @keyframes runBottom {
        0% {
          right: -100%;
        }
        100% {
          right: 100%;
        }
      }

      @keyframes runLeft {
        0% {
          bottom: -100%;
        }
        100% {
          bottom: 100%;
        }
      }

      .product-Items img {
        width: 100%;
        aspect-ratio: 1;
        margin-bottom: 5px;
        border-radius: 5px;
      }

      .product-Items .buy {
        position: absolute;
        top: 0;
        right: 0;
        width: 30px;
        height: 40px;
        transition:
          box-shadow 0.35s ease,
          transform 0.35s ease;

        /* màu nền */
        background: #fff;

        /* cắt hình */
        clip-path: polygon(
          0 5%,
          5% 0,
          95% 0,
          100% 5%,
          100% 100%,
          50% 92%,
          0 100%
        );
      }

      /* viền ngoài */
      .product-Items .buy::before {
        content: "";
        position: absolute;
        inset: 0;
        background: #ccbb51;

        clip-path: polygon(
          0 5%,
          5% 0,
          95% 0,
          100% 5%,
          100% 100%,
          50% 92%,
          0 100%
        );

        z-index: -2;
      }

      /* lớp trong tạo độ dày viền */
      .product-Items .buy::after {
        content: "";
        position: absolute;
        inset: 2px;
        background: #e30e0e;

        clip-path: polygon(
          0 5%,
          5% 0,
          95% 0,
          100% 5%,
          100% 100%,
          50% 92%,
          0 100%
        );

        z-index: -1;
      }

      .product-Items .buy i {
        color: #e9d554;
        font-size: 12px;

        position: absolute;
        top: 50%;
        left: 50%;

        transform: translate(-50%, -50%);

        transition:
          color 0.35s ease,
          font-size 0.35s ease;
      }

      .product-Items .buy:hover {
        box-shadow:
          0 0 5px #e30e0e,
          0 0 15px rgba(227, 14, 14, 0.6);
      }

      .product-Items .buy:hover i {
        color: #d5d0a9;
        font-size: 15px;

        transform: translate(-50%, -50%) scale(1.05);
      }

      .product-Accounts {
        flex: 1;
        min-width: 180px;
        max-width: 480px;
        margin: 0 auto;
        height: auto;
        min-height: 150px;
        background-color: #1c1c1c;
        border-radius: 5px;
        padding: 5px;
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        position: relative;
      }

      .product-Accounts img {
        width: 100%;
        height: auto;
        border: #fff solid 1px;
        border-bottom: none;
        aspect-ratio: 16/9;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
      }

      .product-Accounts .id-acc {
        padding: 5px;
        width: 100%;
        background-color: #911818;
        color: rgb(247, 253, 255);
        font-weight: bold;
        font-size: 15px;
        border: #fff solid 1px;
        border-top: none;
        margin-bottom: 5px;
        border-bottom-left-radius: 5px;
        border-bottom-right-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s ease;
      }
      .product-Accounts .type-acc,
      .product-Accounts .level-acc,
      .product-Accounts .note-acc {
        line-height: 1.2;
        color: #fff;
        font-size: 15px;
      }

      .product-Accounts .btn-acc {
        padding: 5px 10px;
        width: 100%;
        font-size: 12px;
        margin-top: 5px;
        background-color: #007bff;
        color: rgb(247, 253, 255);
        font-weight: bold;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.5s ease;
      }

      .product-Accounts .btn-acc:hover {
        background-color: #0056b3;
      }

      /* overlay */
      .product-Detail {
        display: none;
      }

      .product-Detail.active {
        display: block;
        position: fixed;
        z-index: 9999;
        top: 80px;
        left: 0;
        right: 0;
        bottom: 0;
        width: 100%;
        height: auto;
        min-height: calc(100vh - 80px);
        background: rgb(53, 53, 53);
        overflow-x: scroll;
      }

      /* khung nội dung */
      .product-Details {
        width: 100%;
        padding: 10px clamp(10px, 5%, 50px);
        position: relative;
      }

      /* nút đóng */
      .close-detail {
        position: fixed;
        top: 80px;
        right: 0;
        width: 25px;
        height: 25px;
        border: none;
        border-bottom-left-radius: 20%;
        cursor: pointer;
        font-size: 15px;
        z-index: 10000;
      }

      /* info */
      .detail-info {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
        margin-bottom: 10px;
      }

      .detail-info a {
        flex: 1;
        padding: 5px 10px;
        min-width: 140px;
        border-radius: 5px;
        font-size: 15px;
        font-weight: 500;
        background: #000000;
      }

      .detail-info a span {
        color: #fff;
      }

      /* ảnh */
      .detail-images {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
        align-content: center;
        justify-content: space-between;
        gap: 10px;
      }

      .detail-images img {
        flex: 1;
        max-width: 480px;
        min-width: 360px;
        border-radius: 5px;
        margin: 0 auto;
        aspect-ratio: 16/9;
        cursor: pointer;
      }

      .body-bottom .view {
        display: none;
      }

      .body-bottom .view.active {
        display: flex;
      }

      /* FOOTER */
      .footer {
        width: 100%;
        height: auto;
        min-width: 300px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        background: #2a2a2a;
        align-items: center; /* Căn giữa theo chiều dọc */
        align-content: center;
        justify-content: center; /* Căn giữa theo chiều ngang */
        justify-items: center;
        position: relative;
      }

      .footer .f-left,
      .footer .f-center,
      .footer .f-right {
        min-width: 360px;
        flex: 1;
        height: min-content;
        min-width: 300px;
        margin: 0 auto;
        display: flex;
        align-items: center; /* Căn giữa theo chiều dọc */
        align-content: center;
        justify-content: center; /* Căn giữa theo chiều ngang */
        justify-items: center;
        position: relative;
        flex-direction: column; /* Nếu bạn có nhiều post, vẫn xếp theo dòng */
      }

      .footer span {
        width: 100%;
        height: 30px;
        min-width: 300px;
        margin: 0;
        display: flex;
        padding: 0 15px;
        font-size: 18px;
        font-weight: 600;
        color: white;
        background-color: rgba(67, 67, 67, 0.708);
        justify-content: center; /* Căn giữa theo chiều ngang */
        justify-items: center;
        align-items: left;
        position: relative;
        flex-direction: column; /* Nếu bạn có nhiều post, vẫn xếp theo dòng */
      }

      .footer .f-content {
        width: 100%;
        height: fit-content;
        min-height: 30px;
        min-width: 300px;
        margin: 0;
        display: flex;
        padding: 5px 10px;
        align-items: center; /* Căn giữa theo chiều dọc */
        align-content: center;
        justify-content: center; /* Căn giữa theo chiều ngang */
        justify-items: center;
        position: relative;
        flex-direction: column; /* Nếu bạn có nhiều post, vẫn xếp theo dòng */
      }

      .footer .f-content a {
        color: rgb(195, 195, 195);
        width: 100%;
        display: flex;
        height: 20px;
        font-size: 15px;
        text-decoration: none;
      }

      .footer .f-content a i {
        margin-right: 3px;
        width: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
        justify-items: center;
      }

      .footer .f-content a:hover,
      .footer .f-content a:active {
        color: #ededed;
      }

      @media (max-width: 990px) {
        .footer .f-left,
        .footer .f-center {
          width: calc(100% / 2);
        }

        .footer .f-right {
          width: 100%;
        }
      }

      @media (max-width: 660px) {
        .footer .f-left,
        .footer .f-center,
        .footer .f-right {
          width: 100%;
        }
      }

      /* COPYRIGHT */
      .copyright {
        font-size: 15px;
        text-align: center;
        opacity: 0.8;
        line-height: 1.5;
        color: #c1c1c1; /* xám dịu */
      }
    </style>
  </head>
  <body>
    <!-- Header Logo -->
    <div class="body-top">
      <div class="img">
        <img
          src="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png"
          alt="Background"
        />
      </div>
      <div class="menu">
        <label data-target="introduce"><a>GIỚI THIỆU</a></label>
        <label data-target="items"><a>VẬT PHẨM</a></label>
        <label data-target="account"><a>TÀI KHOẢN</a></label>
      </div>
      <div class="img">
        <img
          src="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png"
          alt="Background"
        />
      </div>
    </div>

    <div class="body-bottom">
      <!-- VIDEO -->
      <div class="video-container introduce view active"></div>
      <script>
        const fixedVideo = "wIBA8s1z_8U";
        let player;

        // load youtube api
        function loadYouTubeAPI() {
          return new Promise((resolve) => {
            if (window.YT && YT.Player) return resolve();

            const tag = document.createElement("script");
            tag.src = "https://www.youtube.com/iframe_api";
            document.body.appendChild(tag);

            window.onYouTubeIframeAPIReady = () => resolve();
          });
        }

        function createPlayer() {
          const container = document.querySelector(".video-container");

          player = new YT.Player(container, {
            videoId: fixedVideo,
            playerVars: {
              autoplay: 1,
              mute: 1,
              controls: 0, // hiện control
              rel: 1,
              modestbranding: 0,
              loop: 1,
              playlist: fixedVideo, // bắt buộc để loop
              fs: 0, // bỏ fullscreen
              iv_load_policy: 3, // bỏ annotation
            },
            events: {
              onReady: (e) => e.target.playVideo(),
            },
          });
        }

        async function init() {
          await loadYouTubeAPI();
          createPlayer();
        }

        init();
      </script>

      <!-- Panel -->
      <img
        src="https://raw.githubusercontent.com/OTVGroup/OTISStore/main/Panel/OTISStore.png"
        alt="Panel/OTISStore"
        class="panel introduce view active"
      />

      <div class="header introduce view active">
        <strong>NEW POST</strong>
      </div>
      <div class="video-content introduce view active" id="playlist"></div>
      <script>
        document.addEventListener("DOMContentLoaded", async () => {
          const channelId = "UCM8xwnvLQ60wfEgduDRzRMg";
          const excludeIds = ["wIBA8s1z_8U"];

          const container = document.getElementById("playlist");

          const url =
            `https://api.rss2json.com/v1/api.json?rss_url=` +
            encodeURIComponent(
              `https://www.youtube.com/feeds/videos.xml?channel_id=${channelId}`,
            );

          try {
            const res = await fetch(url);
            const data = await res.json();

            const videos = data.items
              .filter(
                (video) => !excludeIds.includes(video.link.split("v=")[1]),
              )
              .slice(0, 6);

            videos.forEach((video) => {
              const videoId = video.link.split("v=")[1];

              container.insertAdjacentHTML(
                "beforeend",
                `
                <div class="video-box">
                    <iframe
                        width="100%"
                        height="315"
                        src="https://www.youtube.com/embed/${videoId}"
                        frameborder="0"
                        allowfullscreen>
                    </iframe>
                </div>
                `,
              );
            });
          } catch (err) {
            console.error(err);
          }
        });
      </script>

      <div class="header introduce view active">
        <strong>GROUP FACEBOOK</strong>
      </div>
      <div class="group-content introduce view active">
        <div
          class="group-box"
          onclick="
            window.open(
              'https://www.facebook.com/share/g/1EBEp3fyL2/',
              '_blank',
            )
          "
        >
          <img
            src="https://raw.githubusercontent.com/OTVGroup/OTISStore/main/Background%20-%20Game/Background%20-%20Khu%20Vườn%20Trên%20Mây.jpg"
            alt="Group-Khu_Vườn_Trên_Mây"
          />
          <a>Khu Vườn Trên Mây</a>
        </div>
        <div
          class="group-box"
          onclick="
            window.open(
              'https://www.facebook.com/share/g/1HSyoKB62D/',
              '_blank',
            )
          "
        >
          <img
            src="https://raw.githubusercontent.com/OTVGroup/OTISStore/main/Background%20-%20Game/Background%20-%20Liên%20Quân.jpg"
            alt="Group-Liên_Quân"
          />
          <a>Liên Quân Mobile</a>
        </div>
        <div
          class="group-box"
          onclick="
            window.open(
              'https://www.facebook.com/share/g/15yrvETXAx/',
              '_blank',
            )
          "
        >
          <img
            src="https://raw.githubusercontent.com/OTVGroup/OTISStore/main/Background%20-%20Game/Background%20-%20Clash%20Of%20Clans.jpg"
            alt="Group-Clash_Of_Clans"
          />
          <a>Clash Of Clans</a>
        </div>
        <div
          class="group-box"
          onclick="
            window.open(
              'https://www.facebook.com/share/g/15ipUB67z4/',
              '_blank',
            )
          "
        >
          <img
            src="https://raw.githubusercontent.com/OTVGroup/OTISStore/main/Background%20-%20Game/Background%20-%20Free%20Fire.jpg"
            alt="Group-Free_Fire"
          />
          <a>Free Fire</a>
        </div>
      </div>

      <!-- VẬT PHẨM GAME -->
      <div class="header items view active">
        <strong> VẬT PHẨM KHU VƯỜN TRÊN MÂY </strong>
      </div>
      <!-- List Vật Phẩm - Khu Vườn Trên Mây -->
      <div class="list-item items view active" id="KVTM-items"></div>
      <!-- List Vật Phẩm - Liên Quân Mobile -->
      <!-- <div class="list-item items view active" id="LQM-items"></div> -->
      <!-- List Vật Phẩm - Clash Of Clans -->
      <!-- <div class="list-item items view active" id="COC-items"></div> -->
      <!-- List Vật Phẩm - Free Fire -->
      <!-- <div class="list-item items view active" id="FF-items"></div> -->

      <!-- TÀI KHOẢN GAME -->
      <!-- <div class="header account view">
        <strong> TÀI KHOẢN KHU VƯỜN TRÊN MÂY </strong>
      </div> -->
      <!-- <div class="list-acc account view active" id="KVTM-acc"></div> -->

      <!-- <div class="header account view">
        <strong> TÀI KHOẢN LIÊN QUÂN MOBILE </strong>
      </div> -->
      <!-- <div class="list-acc account view active" id="LQM-acc"></div> -->

      <!-- <div class="header account view">
        <strong> TÀI KHOẢN CLASH OF CLANS </strong>
      </div> -->
      <!-- <div class="list-acc account view active" id="COC-acc"></div> -->
       
      <!-- <div class="header account view">
        <strong> TÀI KHOẢN FREE FIRE </strong>
      </div> -->
      <!-- <div class="list-acc account view active" id="FF-acc"></div> -->
      <div class="list-acc account view">Trống !</div>

      <!-- Footer -->
      <div class="footer">
        <div class="f-left">
          <span class="f-header">OTVGroup</span>
          <div class="f-content">
            <a href="https://maps.app.goo.gl/6Eh4xp7Ainpmf6FZ9" target="_blank">
              <i class="fas fa-map-marker-alt"></i>Ho Chi Minh, Viet Nam
            </a>
            <a href="mailto:otvgroupcontact@gmail.com" target="_blank">
              <i class="fas fa-envelope"></i>otvgroupcontact@gmail.com
            </a>
            <a href="tel:+84329022431" target="_blank">
              <i class="fa fa-phone"></i>+84 329 022 431
            </a>
          </div>
        </div>

        <div class="f-center">
          <span class="f-header">LIÊN KẾT</span>
          <div class="f-content">
            <a href="https://www.facebook.com/OTV.OTISStore" target="_blank">
              <i class="fab fa-facebook-f"></i>Facebook
            </a>
            <a href="https://www.youtube.com/@otisstorevn" target="_blank">
              <i class="fab fa-youtube"></i>YouTube
            </a>
            <a href="https://www.tiktok.com/@otisstore.vn" target="_blank">
              <i class="fab fa-tiktok"></i>Tik Tok
            </a>
          </div>
        </div>

        <div class="f-right">
          <span class="f-header">THANH TOÁN</span>
          <div class="f-content">
            <a
              href="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Donate/Momo.jpg"
              target="_blank"
              style="
                text-decoration: none;
                transition: 0.3s;
                padding-left: 10px;
              "
              onmouseover="this.style.color = '#fd00c2'"
              onmouseout="this.style.color = ''"
              >Momo</a
            >
            <a
              href="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Donate/ZaloPay.jpg"
              target="_blank"
              style="
                text-decoration: none;
                transition: 0.3s;
                padding-left: 10px;
              "
              onmouseover="this.style.color = '#00a2ff'"
              onmouseout="this.style.color = ''"
              >ZaloPay</a
            >
            <a
              href="https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Donate/Agribank.jpg"
              target="_blank"
              style="
                text-decoration: none;
                transition: 0.3s;
                padding-left: 10px;
              "
              onmouseover="this.style.color = '#c00000'"
              onmouseout="this.style.color = ''"
              >Agribank</a
            >
          </div>
        </div>
      </div>

      <!-- Copyright -->
      <div class="copyright">
        © <span id="year"></span> OTISStore. Tất cả các quyền được bảo lưu.
      </div>
    </div>

    <!-- List Detail - Khu Vườn Trên Mây -->
    <div class="product-Detail" id="productDetail"></div>

    // DATA GAME
    <script>
      const dataItems = {
        KVTM: [
          // VP.KVTM
          // Sấy 1
          // Nước Ép 1
          {
            name: "Nước Nho",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/68.png",
            price: "100",
            quantity: "1",
          },
          // Vải 2
          {
            name: "Vải Trắng",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/83.png",
            price: "70",
            quantity: "1",
          },
          {
            name: "Vải Đen",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/85.png",
            price: "70",
            quantity: "1",
          },
          // Ngọc 0
          // Tinh Dầu 0
          // Trà 3
          {
            name: "Trà Nho",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/101.png",
            price: "60",
            quantity: "1",
          },
          {
            name: "Trà Hoa Cúc",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/94.png",
            price: "55",
            quantity: "1",
          },
          {
            name: "Trà Trái Cây",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/96.png",
            price: "50",
            quantity: "1",
          },
          // Hoa Tươi 1
          {
            name: "Bó Cúc",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Items%20-%20KVTM/89.png",
            price: "50",
            quantity: "1",
          },
          // Nước Hoa 0
          // Túi Hương 0
          // Vật Phẩm May 1
          // Hạt Giống 8
          {
            name: "Nho",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Plant%20-%20KVTM/29.png",
            price: "500",
            quantity: "1",
          },
          {
            name: "Lài",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Plant%20-%20KVTM/30.png",
            price: "500",
            quantity: "1",
          },
          {
            name: "Cúc",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Plant%20-%20KVTM/32.png",
            price: "400",
            quantity: "1",
          },
          // Bọ 0
          // Vật Phẩm Khác 2
          {
            name: "Vợt Trắng",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Other%20-%20KVTM/15.png",
            price: "80",
            quantity: "1",
          },
          {
            name: "Vợt Xanh",
            image:
              "https://raw.githubusercontent.com/OTVGroup/OTISStore/main/KVTM/Other%20-%20KVTM/16.png",
            price: "80",
            quantity: "1",
          },
          // Vàng & Vật Phẩm Sự Kiện 1
        ],
        LQM: [],
        COC: [],
        FF: [],
      };

      const dataAccounts = {
        KVTM: [
          {
            id: "###-###-###",
            type: "###-###",
            level: "###",
            note: "Trống!",
            img: [
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
            ],
          },
        ],
        LQM: [],
        COC: [],
        FF: [],
      };

      // HÀM RENDER Items
      function renderItems(id, list) {
        const containerItems = document.getElementById(id);
        if (!containerItems) return;

        let html = "";

        list.forEach((item) => {
          const img =
            item.img ||
            item.image ||
            item.link ||
            item.url ||
            (item.items && item.items[0]?.img) ||
            "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png";

          html += `
              <div class="product-Items">
                <img src="${img}" alt="${item.name || "No name"}">
                <a>Tên: ${item.name || "Không có tên"}</a>
                <p>SL: ${(item.price || 0).toLocaleString()} / ${item.quantity === 0 ? "Hết hàng" : "Còn: x" + (item.quantity ?? 0)}</p>
                <span class="top" style="--color: #d7ce92;"></span>
                <span class="right" style="--color: #d7ce92;"></span>
                <span class="bottom" style="--color: #d7ce92;"></span>
                <span class="left" style="--color: #d7ce92;"></span>
                <div class="buy" onclick="window.open('https://www.facebook.com/OTV.OTISStore', '_blank')">
                  <i class="fa-solid fa-cart-shopping"></i>
                </div>
              </div>
            `;
        });

        containerItems.innerHTML = html;
      }

      // HÀM RENDER Accounts
      function renderAccounts(id, list) {
        const containerAccounts = document.getElementById(id);
        if (!containerAccounts) return;
        let html = "";
        list.forEach((item, index) => {
          /* lấy ảnh đầu tiên */
          let firstImg = "";
          if (Array.isArray(item.img)) {
            firstImg = item.img[0];
          } else if (typeof item.img === "string") {
            firstImg = item.img.split(",")[0].trim();
          }

          /* fallback */
          const img =
            firstImg && firstImg !== ""
              ? firstImg
              : "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png";

          html += `
                <div class="product-Accounts">
                  <img src="${img}" alt="${item.id}" />
                  <div class="id-acc">Mã: ${item.id}</div>
                  <div class="type-acc">Phân Loại: ${item.type}</div>
                  <div class="level-acc">Cấp Độ: ${item.level}</div>
                  <div class="note-acc">Ghi Chú: ${item.note}</div>
                  <button class="btn-acc" data-index="${index}">
                    Xem Chi Tiết !
                  </button>
                </div>
              `;
        });

        containerAccounts.innerHTML = html;

        containerAccounts.querySelectorAll(".btn-acc").forEach((btn) => {
          btn.addEventListener("click", function () {
            const index = this.dataset.index;
            renderDetails("productDetail", [list[index]]);
          });
        });
      }

      // HÀM RENDER Details Account
      function renderDetails(id, list) {
        const containerDetails = document.getElementById(id);
        if (!containerDetails) return;

        let html = "";

        list.forEach((item) => {
          let imgs = [];

          if (Array.isArray(item.img)) {
            imgs = item.img;
          } else if (typeof item.img === "string") {
            imgs = item.img ? item.img.split(",").map((i) => i.trim()) : [];
          }

          if (!imgs.length) {
            imgs = [
              "https://raw.githubusercontent.com/OTVGroup/OTVGroup/main/Picture/Avatar%20-%20OTISStore.png",
            ];
          }

          html += `
            <div class="product-Details">
              <button class="close-detail">✕</button>
              <div class="detail-info">
                <a class="id-acc" style="color: red;">
                  <span>Mã:</span> ${item.id}
                </a>
                <a class="type-acc" style="color: blue;">
                  <span>Phân Loại:</span> ${item.type}
                </a>
                <a class="level-acc" style="color: green;">
                  <span>Cấp Độ:</span> ${item.level}
                </a>
                <a class="note-acc" style="color: yellow;">
                  <span>Ghi Chú:</span> ${item.note}
                </a>
              </div>
              <div class="detail-images">
                ${imgs
                  .map(
                    (img) => `
                  <img src="${img}" alt="${item.id}">
                `,
                  )
                  .join("")}
              </div>
            </div>
          `;
        });

        containerDetails.innerHTML = html;
        containerDetails.classList.add("active");

        // nút đóng
        containerDetails
          .querySelector(".close-detail")
          .addEventListener("click", closeDetail);
      }

      function closeDetail() {
        document.getElementById("productDetail").classList.remove("active");
      }

      // GỌI RENDER
      renderItems("KVTM-items", dataItems.KVTM);
      renderItems("LQM-items", dataItems.LQM);
      renderItems("COC-items", dataItems.COC);
      renderItems("FF-items", dataItems.FF);
      renderAccounts("KVTM-acc", dataAccounts.KVTM);
      renderAccounts("LQM-acc", dataAccounts.LQM);
      renderAccounts("COC-acc", dataAccounts.COC);
      renderAccounts("FF-acc", dataAccounts.FF);
    </script>

    // ACTIVE MENU
    <script>
      const labels = document.querySelectorAll(".menu label");
      labels.forEach((label) => {
        label.addEventListener("click", () => {
          const target = label.dataset.target;
          // active menu
          labels.forEach((l) => l.classList.remove("active"));
          label.classList.add("active");
          // show nội dung
          document
            .querySelectorAll(".view")
            .forEach((v) => v.classList.remove("active"));
          document
            .querySelectorAll("." + target)
            .forEach((v) => v.classList.add("active"));
        });
      });
    </script>
  </body>
</html>
