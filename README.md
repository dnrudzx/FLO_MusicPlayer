# FLO_MusicPlayer
프로그래머스 과제관 
안드로이드 뮤직 플레이어 앱

STEP 1. 프로젝트 요구사항


  언어 : Java, Kotlin 중 택1
  
  sdk Version : 
    minSdkVersion : 21
    targetSdkVersion : 27이상
    
  라이브러리 사용 : 필요시 외부라이브러리 사용 가능, 사용시 출처 표시
  
  
  화면구성 : 
  
    스플래시 스크린
    
    음악 재생화면 : 재생 중인 음악 정보(제목, 가수, 앨범 커버 이미지, 앨범명)
                    현재 재생중인 부분의 가사 하이라이팅
                    Seekbar
                    Play/Stop 버튼
                    
    전체 가사 보기 화면 : 특정 가사로 이동할 수 있는 토글 버튼
                    전체 가사 화면 닫기 버튼
                    Seekbar
                    Play/Stop 버튼

  기능 요구사항 : 
  
    스플래시 스크린 : 제공되는 이미지를 2초간 노출 -> 음악 재생화면으로 전환
    
    음악 재생화면 : 주어진 노래의 재생화면 노출(앨범 커버이미지, 앨범명, 아티스트명, 곡명)
                    재생버튼을 누르면 음악이 재생(1개의 음악파일 제공)
                        재생시 현재 재생되는 구간대의 가사가 실시간으로 표시
                    정지버튼을 누르면 재생중이던 음악 정지
                    SeekBar를 조작하여 재생 시작지점 이동
                    
    전체 가사 보기 화면 : 전체 가사가 띄워진 화면이 있고, 특정 가사부분으로 이동할 수 있는 토글버튼 존재
                        토글버튼 ON : 특정 가사 터치시 해당 구간부터 재생
                        토글버튼 OFF : 특정 가사 터치시 전체 가사 화면 닫기
                    전체 가사 화면 닫기 버튼
                    현재 재생중인 부분의 가사가 하이라아팅
         
         
  제공되는 음원 : https://grepp-programmers-challenges.s3.ap-northeast-2.amazonaws.com/2020-flo/song.json
  
      제공하는 json파일의 내용 변경시 앱에서 반영하여 새로운 곡 표시
      
      json파일 필드 :
              singer : 아티스트명
              album : 앨범명
              title : 곡명
              image : 앨범 커버 이미지
              file : mp3파일 링크
              lyrics : 시간으로 구분 된 가사. 가사의 각 줄 마다 해당 가사가 표시되기 시작되어야 할 시간이 분:초:밀리초 단위로 적혀 있으며, 이를 활용하여 현재 재생되는 곡의 가사를 표시해야 합니다.
