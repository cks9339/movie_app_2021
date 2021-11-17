

## 김민혁 201640208

### [ 11월 17일]
<pre>
<code>
HandleChange(e){
    this.setState({text:e.target.value})
}
HandleSubmit(e){ 
    e.preventDefault()
    if (this.state.text.length ===0){
        return 
    }
    const newItem = {
        text: this.state.text,
        id: Date.now()
    } 
    this.setState(state => ({
        items: state.items.concat(newItem), 
        text: ''
    }))    
}
</code>
</pre>
### HandleSubmit(e)에서 e.preventDefault() 메소드를 사용하는 이유는?
브라우저에서 양식을 제출할 때는 기본적으로 브라우저의 새로 고침이 발생하는데, React나
SPA의 경우 필요가 없는 동작임으로 이를 방지하기 위해 사용한다.
1. stae.text의 길이가 0이면 아무 것도 반환하지 않는다.
2. 0이 아니면 newitem에 입력 받은 text와 현재 시간을 저장한다.
3. 현재 시간은 왜 저장하는 걸까? 조금 생각해 보자.
4. 이렇게 저장된 newitem을 state의 item배열에 저장하고 , text를 비운다.


[ 11월 3일]

네비게이션 만들어 보기
* 액션01. Navigaition 컴포넌트 만들기
* 액션02. Navigaition 컴포넌트 App 컴포넌트에 포함시키기
* 액션03. Home 링크 눌러 보기
* 액션04. a 태그 Link 컴포넌트로 바꾸기
* 액션05. Navigation 컴포넌트 위치 다시 확인하기
* 액션06. Navigation 컴포넌트 스타일링하기

영화 상세 정보 기능 만들어 보기
* 액션01. route props 살펴보기
* 액션02. route props에 데이터 담아 보내기
* 액션03. route props 다시 살펴 보기
* 액션04. Navigation 컴포넌트 정리하기
* 액션05. Movie 컴포넌트에 Link 컴포넌트 추가하기
* 액션06. Detail 컴포넌트 만들기
* 액션07. Route 컴포넌트 추가하기
* 액션08. 영화 카드를 눌러 /movie-detail로 이동한 다음 영화 데이터 확인하기
* 액션09. /moive-detail로 바로 이동하기

리다이렉트 기능 만들어보기
* 액션01. History 키 살펴보기
* 액션02. Detail 컴포넌트 클래스형 컴포넌트로 변경하기
* 액션03. push() 함수 사용하기
* 액션04. 리다이렉트 기능 확인해 보기
* 액션05. 영화 제목 출력하기
* 액션06. /moive-detail로 바로 이동하기
* 액션07. location.state 확인하기


[ 10월 27일]


영화 앱에 여러 기능 추가하기
* react-router-dom 설치하고 프로젝트 폴더 정리하기
    * 액션01. react-router-dom 설치
    * 액션02. components 폴더에 Movive 컴포넌트 옮기기
    * 액션03. routes 폴더에 라우터가 보여줄 화면 만들기
    * 액션04. Home.js 수정하기 
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
