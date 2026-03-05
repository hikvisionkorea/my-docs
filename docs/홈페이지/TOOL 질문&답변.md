\# 문의 답변


# 🛠️ 문의 답변

??? success "VLC 플레이어를 통한 멀티캐스트 영상 수신 방법"
    **설정 방법:**<br>
    - rtsp://<username>:<password>@<IP address>:<RTSP port>/ISAPI/streaming/channels/101?transportmode=multicast<br>
    - VLC 설정 -> 입력/코덱 -> Demuxer -> RTP/RTSP의 'RTSP를 통한 RTP 멀티캐스트 강제 선택' 체크

??? success "Local Playback 영상 검색되지 않습니다. NO VIDEO FILE FOUND "
    **답변:** remote backup 활용 권장<br>
                 같은망 PC에 녹화기 영상 수동 / 자동 백업 프로그램

??? success "VLC 플레이어에서 RTSP스트림 요청시 영상이 안나오는 문제"
    **답변:** 녹화기 HC 설정중 스트림 암호화 기능이 활성화된 경우 해당증상 발생, 스트림 암호화 기능 해제시 정상 동작

??? success "카메라에서 송출하는 멀티캐스트 스트림을 PC VLC에서 확인하는 방법"
    **답변:** Web 페이지에서 멀티캐스트 사용 설정 및 <br>
                 아래 명령어 사용하면 VLC에서 멀티캐스트 스트림 요청시<br>
                 카메라에서 멀티캐스트 주소로 스트림 송신<br>
                  rtsp://카메라ID:카메라PW@카메라IP:RTSP 포트/ISAPI/streaming/channels/101?transportmode=multicast

??? success "리모트 백업프로그램 사용하여 백업시 사진처럼 채널명 대신 33 34 35 이런식으로 되어있는데 의미랑 임의 설정 가능한지 확인"
    **답변:** 33 --> 1ch1<br>
                 34--> 2ch<br>
                 이런 순서로 저장됨, 임의 설정 불가능

??? success "Internet Explorer 종료로 인해 Edge 브라우저에서 설정"
    **답변:** 해당 링크를 클릭해주세요 [엣지 브라우저 영상 보기 방법 PDF 바로가기](./docs/엣지 브라우저 영상 보기 방법.pdf)


---



