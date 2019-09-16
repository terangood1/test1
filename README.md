# 비쥬얼 프로그래밍 과제
 ## 간단한 MFC 
 
 ### visual studio 2019 사용  
 
 #### 두 수를 더하는 프로그램 1
 
<img src= "https://user-images.githubusercontent.com/54833169/64945719-2a781c80-d8ac-11e9-9510-a1e66ea1a8ad.PNG" width="300">
 
  #### 1
  새 프로젝트 만들기를 선택 

<img src="https://user-images.githubusercontent.com/54833169/64946391-bb9bc300-d8ad-11e9-9f32-7650fc80f6e9.PNG" width="300">
 
 #### 2
검색에 mfc 검색 후 mfc앱 선택 후 다음버튼을 누른다. mfc가 안나오는 경우는 설치가 안되있는 경우 다시 설치를 해준다.
 
 <img src="https://user-images.githubusercontent.com/54833169/64946417-ca827580-d8ad-11e9-9631-f88d80faa93a.PNG" width="500">
  
  #### 3
  프로젝트 이름은 입력 한 후 솔루션 및 프로젝트를 같은 디렉터리에 배치를 체크 해준다음 만들기를 클릭한다.

![4](https://user-images.githubusercontent.com/54833169/64946418-ca827580-d8ad-11e9-93bc-e0572c7da3aa.PNG)
 
  #### 4
  애플리케이션 종류 탭에서 **대화 상자 기반** 으로 바꿔준다
 
<img src="https://user-images.githubusercontent.com/54833169/64949268-c6f1ed00-d8b3-11e9-9778-3998cc3ed536.PNG" width="600">

 #### 5
 완료 화면 

![5](https://user-images.githubusercontent.com/54833169/64946419-ca827580-d8ad-11e9-8df6-5026d58ee591.PNG)

 #### 6
 오른쪽 솔루션 탐색기 탭에 있는 리소스 파일을 열고 프로젝트명.rc를 더블 클릭한다.

![6](https://user-images.githubusercontent.com/54833169/64946420-cb1b0c00-d8ad-11e9-8c14-c17629444d6d.PNG)
 
 #### 7
 그 후 나오는 창에서 Dialog를 클릭 한뒤 IDD_프로젝트명_DIALOG를 더블 클릭한다.

<img src="https://user-images.githubusercontent.com/54833169/64946421-cb1b0c00-d8ad-11e9-8c20-ffa0b303c36e.PNG" width="600">
 
 #### 8
 완료 화면 

![8](https://user-images.githubusercontent.com/54833169/64946422-cb1b0c00-d8ad-11e9-8ca7-6ef4a53833ed.PNG)

 #### 9
 화면 왼쪽에 있는 **대화 상자 편집기**에서 **Edit Control**를 클릭 후 끌어서 프로그램 창에 놓는다.

![9](https://user-images.githubusercontent.com/54833169/64946423-cb1b0c00-d8ad-11e9-9f7f-ac0eb503fd33.PNG)

 #### 10
 같은 방식으로 **Button**을 끌어서 놓는다. 

![10](https://user-images.githubusercontent.com/54833169/64946424-cbb3a280-d8ad-11e9-8d22-e72daf0298c5.PNG)

 #### 11
 Edit Control을 3개 Button을 1개 위치를 잡아 준 뒤 생성한 Button1을 더블클릭 해준다.
 
 ![11](https://user-images.githubusercontent.com/54833169/64946425-cbb3a280-d8ad-11e9-92bb-09423c554f10.PNG)
 
 #### 12
 더블 클릭을 하면 사진 처럼 코드를 입력할 수 있는 화면이 나온다. **void C프로젝트명Dlg::OnBnClickedButton1()** 이 생성 되었는지를 확인 

![12](https://user-images.githubusercontent.com/54833169/64946426-cbb3a280-d8ad-11e9-9c37-2391a558a7f6.PNG)

 #### 13
 `int a = GetDlgItemInt(IDC_EDIT1);` 을 입력한다. 

![13](https://user-images.githubusercontent.com/54833169/64946411-c9514880-d8ad-11e9-8c23-d735e999d0e7.PNG)

 #### 14
 **IDC_EDIT1** 은 생성한 **Edit Control**을 클릭하면 오른쪽 하단에 **ID탭**에 있는 이름과 같은 것을 써준다. 

![14](https://user-images.githubusercontent.com/54833169/64946412-c9e9df00-d8ad-11e9-9040-74dafafb2aae.PNG)

 #### 15
 `int b = GetDlgItemInt(IDC_EDIT2);` 를 입력한 뒤 `int c = a+b;` 를 입력해준다. **Edit Control**에 두 수를 넣으면 버튼을 클릭 했을 때 더  한 값을 출력 하기 위해 더해지는 두 수를 받아 올 수 있게 하는 코드이다. **int c = a+b;** 경우는 두 수를 더한 값을 저장하는 코드이다.

![15](https://user-images.githubusercontent.com/54833169/64946413-c9e9df00-d8ad-11e9-992a-f8fcf497543a.PNG)

 #### 16
 `SetDlgItemInt(IDC_EDIT3, c);` 입력한다. 더해진 값 **c** 를 프로그램 창에 넣은 **Edit Control** 의 마지막 부분에 출력해주는 코드이다. 

 ![16](https://user-images.githubusercontent.com/54833169/64946414-c9e9df00-d8ad-11e9-880f-47b64c4407e1.PNG)
 
 #### 17
 입력을 완료 한 후 **로컬 Windows 디버거**를 클릭한다.

![17](https://user-images.githubusercontent.com/54833169/64946415-ca827580-d8ad-11e9-9b73-4012c4e6ea6b.PNG)

 #### 18
 새로 뜨는 창에서 위에 두 칸에 수를 입력 한 후 버튼을 누르면 더한 값이 밑에 칸에 나온다.
 
 
 #### 두 수를 더하는 프로그램 2
