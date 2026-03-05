<style>
    /* === 기본 레이아웃 === */
    #vanta-bg {
        width: 100%;
        height: 600px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        border-radius: 20px;
        background: radial-gradient(circle at center, #0a1b35 0%, #020408 100%);
        position: relative;
        overflow: hidden;
        box-shadow: 0 30px 60px rgba(0,0,0,0.8);
        perspective: 2000px;
    }

    .content-wrapper {
        z-index: 10;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transform-style: preserve-3d;
    }

    /* === 🚀 6면 HIKVISION 통합 사이버네틱 큐브 🚀 === */
    .digital-cube {
        width: 160px;
        height: 160px;
        position: relative;
        transform-style: preserve-3d;
        animation: rotateCyberCube 20s infinite linear;
        margin-bottom: 60px;
    }

    /* 내부 발광 코어 */
    .cube-core {
        position: absolute;
        width: 60px; height: 60px;
        top: 50px; left: 50px;
        background: #3fbbef;
        border-radius: 50%;
        filter: blur(25px);
        box-shadow: 0 0 50px #3fbbef;
        opacity: 0.7;
        animation: pulseEnergy 2s infinite ease-in-out;
    }

    .cube-face {
        position: absolute;
        width: 160px;
        height: 160px;
        display: flex;
        align-items: center;
        justify-content: center;
        box-sizing: border-box;
        /* 사이버네틱 그리드 배경 */
        background: 
            linear-gradient(rgba(63, 187, 239, 0.1) 1px, transparent 1px),
            linear-gradient(90deg, rgba(63, 187, 239, 0.1) 1px, transparent 1px),
            rgba(10, 25, 47, 0.8);
        background-size: 20px 20px;
        border: 1px solid rgba(63, 187, 239, 0.4);
        backdrop-filter: blur(8px);
        overflow: hidden;
    }

    /* 코너 브래킷 프레임 */
    .cube-face::after {
        content: '';
        position: absolute;
        inset: 0;
        border: 2px solid #3fbbef;
        clip-path: polygon(
            0 0, 25% 0, 25% 2%, 2% 2%, 2% 25%, 0 25%,
            0 75%, 2% 75%, 2% 98%, 25% 98%, 25% 100%, 0 100%,
            100% 100%, 75% 100%, 75% 98%, 98% 98%, 98% 75%, 100% 75%,
            100% 25%, 98% 25%, 98% 2%, 75% 2%, 75% 0, 100% 0
        );
        box-shadow: 0 0 15px rgba(63, 187, 239, 0.5);
    }

    /* 텍스트 디자인 (홀로그램 스타일) */
    .cube-face span {
        font-family: 'Courier New', monospace;
        font-weight: 900;
        font-size: 18px;
        color: #fff;
        text-shadow: 0 0 10px #3fbbef, 0 0 20px rgba(63, 187, 239, 0.5);
        z-index: 2;
        transform: translateZ(10px); /* 텍스트 돌출 */
    }

    /* 면 조립 */
    .face-front  { transform: translateZ(80px); }
    .face-back   { transform: rotateY(180deg) translateZ(80px); }
    .face-right  { transform: rotateY(90deg) translateZ(80px); }
    .face-left   { transform: rotateY(-90deg) translateZ(80px); }
    .face-top    { transform: rotateX(90deg) translateZ(80px); }
    .face-bottom { transform: rotateX(-90deg) translateZ(80px); }

    /* 애니메이션 */
    @keyframes rotateCyberCube {
        0%   { transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg); }
        100% { transform: rotateX(360deg) rotateY(720deg) rotateZ(360deg); }
    }
    @keyframes pulseEnergy {
        0%, 100% { transform: scale(1); opacity: 0.5; }
        50% { transform: scale(1.5); opacity: 0.8; }
    }

    /* 하단 텍스트 */
    .sub-title {
        font-size: 2.5rem;
        font-weight: 800;
        text-shadow: 0 0 25px rgba(63, 187, 239, 0.8);
        margin-top: 20px;
    }
</style>

<div id="vanta-bg">
    <div class="content-wrapper">
        <img src="logo.png" style="width:160px; margin-bottom:50px; filter: drop-shadow(0 0 10px #3fbbef);" alt="HIKVISION">
        
        <div class="digital-cube">
            <div class="cube-core"></div>
            
            <div class="cube-face face-front"><span>HIKVISION</span></div>
            <div class="cube-face face-back"><span>HIKVISION</span></div>
            <div class="cube-face face-right"><span>HIKVISION</span></div>
            <div class="cube-face face-left"><span>HIKVISION</span></div>
            <div class="cube-face face-top"><span>HIKVISION</span></div>
            <div class="cube-face face-bottom"><span>HIKVISION</span></div>
        </div>
        
        <p class="sub-title">기술 지원 센터</p>
    </div>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r121/three.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/vanta@latest/dist/vanta.net.min.js"></script>

<script>
    // VANTA 배경 애니메이션 설정
    VANTA.NET({
        el: "#vanta-bg",
        mouseControls: true,
        touchControls: true,
        gyroControls: false,
        color: 0x3fbbef,
        backgroundColor: 0x020408,
        points: 14.00,
        maxDistance: 20.00,
        spacing: 16.00
    });
</script>

## 📞 고객 지원 안내 📞1811-5998

**HIKVISION 기술 지원센터에 오신 것을 환영합니다.**

하이크비전에서는 좀 더 다양한 서비스를 제공하기 위해 서비스 홈페이지 및 콜센터를 운영하고 있습니다.<br>



✅콜센터  / 업무시간 : 오전 9시~ 12시, 점심시간 (12시~ 13시) , 13시~ 17시 30분

제품 사용중에 문제가 발생하실경우 1811-5998 콜센터로 문의 부탁드립니다.

오후에는 전화가 몰리는 상황으로 통화가 어려울 수 있습니다.<br>


 

✅하이크비전코리아 카카오톡 상담 문의 카카오톡 채널  /  업무시간 오전 10시~ 12시, (점심시간) 12시~13시, 13시~17시

 **카카오톡 상담 링크 : http://pf.kakao.com/\_xdBded/chat**<br>



🔷문의시 필수 확인 사항

\-    제품 모델명 및 시리얼 번호

\-    제품 펌웨어 정보

\-    현재 접속 가능한 외부 IP 주소.



🔷원격 요청전 필수사항

\-      장치의 비밀번호를 꼭 확인해주시고 원격을 요청해주셔야 합니다.

(공유기 비밀번호도 꼭 알아 놓으셔야 합니다.)

\-      공유기에 PC,녹화기가 연결이 되어 있는지 꼭 확인을 해주셔야 합니다.

