## 김민혁 201640208

[ 10월 27일]


영화 앱에 여러 기능 추가하기
* react-router-dom 설치하고 프로젝트 폴더 정리하기
    * 액션01. react-router-dom 설치
    * 액션02. components 폴더에 Movive 컴포넌트 옮기기
    * 액션03. routes 폴더에 라우터가 보여줄 화면 만들기
    * 액션04. Home.js 수정하기
    * 액션05. Home.css 만들기
    * 액션06. App.js 수정하기
   

* 라우터 만들어 보기
    * 액션01. HashRouter와 Router컴포넌트
    * 액션02. Route 컴포넌트에 phat,component props 추가하기
    * 액션03 About.js 수정하기
     ```
    function About(props) {
        console.og{props};
        return (
            <div className="about-container">
            <span> 앱의설명~</span>
            <span> 자기소개</span>
        )
    }
    export default About
 
 그 후 액션 11까지 진행.
 * 네비게이션 만들어 보기
 * 영화 상세 정보 기능 만들어 보기
 * 리다이렉트 기능 만들어 보기