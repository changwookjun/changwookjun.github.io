<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>팀 소개</title>
  <style>
    :root {
      --bg: #f7f7f7;
      --card-bg: #ffffff;
      --text-main: #111111;
      --text-sub: #666666;
      --border: #e5e5e5;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, "Pretendard",
        system-ui, sans-serif;
      background: var(--bg);
      color: var(--text-main);
      line-height: 1.6;
    }

    .page {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      padding: 40px 16px;
    }

    .container {
      width: 100%;
      max-width: 960px;
      background: var(--card-bg);
      border-radius: 24px;
      padding: 40px 24px 48px;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.05);
    }

    .title-area {
      text-align: center;
      margin-bottom: 40px;
    }

    .title-area h1 {
      font-size: 32px;
      letter-spacing: 0.06em;
      margin-bottom: 10px;
    }

    .title-area p {
      font-size: 15px;
      color: var(--text-sub);
    }

    .team-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 40px 32px;
    }

    .member {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    .member-photo-wrap {
      width: 160px;
      height: 160px;
      border-radius: 50%;
      overflow: hidden;
      margin-bottom: 18px;
      background: #ddd;
    }

    .member-photo {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
    }

    .member-name {
      font-size: 20px;
      font-weight: 700;
      margin-bottom: 4px;
    }

    .member-role {
      font-size: 14px;
      color: var(--text-sub);
      margin-bottom: 10px;
    }

    .member-desc {
      font-size: 13px;
      color: #444;
      max-width: 260px;
    }

    /* 작은 화면 대응 */
    @media (max-width: 720px) {
      .container {
        padding: 28px 18px 32px;
        border-radius: 18px;
      }

      .title-area h1 {
        font-size: 26px;
      }

      .team-grid {
        grid-template-columns: 1fr;
        gap: 32px;
      }

      .member-photo-wrap {
        width: 140px;
        height: 140px;
      }
    }
  </style>
</head>
<body>
  <div class="page">
    <main class="container">
      <header class="title-area">
        <h1>팀 소개</h1>
        <p>배움에 진심인, 든든한 네 명의 팀원을 소개합니다.</p>
      </header>

      <section class="team-grid">
        <!-- 1. 김민서 -->
        <article class="member">
          <div class="member-photo-wrap">
            <!-- 실제 팀원 사진으로 교체하세요 -->
            <img src="img/minseo.jpg" alt="김민서 프로필 사진" class="member-photo" />
          </div>
          <h2 class="member-name">김민서</h2>
          <p class="member-role">교육 · 콘텐츠 기획</p>
          <p class="member-desc">
            유아·초등 교육 콘텐츠를 설계하고, 수업과 연결되는 다양한
            프로젝트형 활동을 기획합니다.
          </p>
        </article>

        <!-- 2. 이수현 -->
        <article class="member">
          <div class="member-photo-wrap">
            <img src="img/soohyun.jpg" alt="이수현 프로필 사진" class="member-photo" />
          </div>
          <h2 class="member-name">이수현</h2>
          <p class="member-role">강사</p>
          <p class="member-desc">
            글쓰기와 인문학 강의를 중심으로, 아이들이 스스로 생각을
            표현할 수 있도록 돕습니다.
          </p>
        </article>

        <!-- 3. 박기웅 -->
        <article class="member">
          <div class="member-photo-wrap">
            <img src="img/kiwoong.jpg" alt="박기웅 프로필 사진" class="member-photo" />
          </div>
          <h2 class="member-name">박기웅</h2>
          <p class="member-role">UX 디자이너</p>
          <p class="member-desc">
            에듀테크 서비스의 UX를 설계하며, 학습자가 쓰기 편한 화면과
            흐름을 만드는 데 집중합니다.
          </p>
        </article>

        <!-- 4. 정다은 -->
        <article class="member">
          <div class="member-photo-wrap">
            <img src="img/daeun.jpg" alt="정다은 프로필 사진" class="member-photo" />
          </div>
          <h2 class="member-name">정다은</h2>
          <p class="member-role">영상 콘텐츠 제작</p>
          <p class="member-desc">
            교육 현장을 담은 영상과 홍보 콘텐츠를 제작하며,
            수업의 분위기와 메시지를 영상으로 전합니다.
          </p>
        </article>
      </section>
    </main>
  </div>
</body>
</html>

