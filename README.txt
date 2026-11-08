배포 방법 (무료 정적 호스팅)

이 폴더 전체가 서비스입니다. 서버 프로그램이 필요 없습니다.
  index.html  서비스 본체 (입력은 사용자 브라우저에만 저장)
  fonts.css   글꼴 (캐시되어 두 번째 방문부터 빠름)
  _headers    보안 헤더 (Cloudflare Pages, Netlify에서 인식)
  robots.txt  검색 노출 차단 (시범 기간)

Cloudflare Pages: 대시보드 > Workers & Pages > Create > Pages > Upload assets 에서 이 폴더를 끌어다 놓기.
Netlify: Sites > Add new site > Deploy manually 에서 이 폴더를 끌어다 놓기.
GitHub Pages: 이 폴더 내용을 저장소에 올리고 Settings > Pages 에서 켜기 (_headers는 적용되지 않음).
자체 서버: 이 폴더를 nginx 등 웹 루트에 복사. HTTPS 필수.

공개 범위: 링크를 아는 사람만 쓰는 시범 운영이면 robots.txt와 noindex를 그대로 두세요.
정식 공개 때는 robots.txt를 지우고 index.html의 noindex 메타를 빼세요.
