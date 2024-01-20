# 객체지향프로그래밍 과제 _ 수강신청 프로그램

수강 신청 프로그램을 사용하는 멤버는 총 세 개다. 
- 강의실, 교수, 학생. 

## 1. 강의실 :
강의실에서는 해당 강의실에 배정된 강의 과목, 시간, 교수를 확인할 수 있음.

## 2. 교수 : 
강의 과목 이름과 시간, 강의실을 입력하여 강의를 추가할 수 있으며, 본인이 추가한 과목에 수강 신청을 한 학생 명단을 확인할 수 있다. 또한, 본인의 강의를 삭제할 수 있다.

## 3. 학생 : 
본인이 수강신청한 과목에 대한 정보(과목명,시간, 교수, 강의실)을 확인할 수 있다. 또한, 수강 신청 작업 및 수강 신청 취소 작업을 할 수 있다.

# 실행 화면
먼저 강의실을 생성한다. (강의실 이름, 최대정원) - 6개

_ex - (혜화관1호,50) (혜화관2호,50) (명진관1호,30) (명진관2호,40) (학림관1호,70) (학림관2호,80)_
![image](https://github.com/Ninky0/classRegistration/assets/113659622/a8044ae4-98e5-4c4a-8e4f-2db5d3412f56)

교수 생성를 생성한다. (교수 이름) - 3명
_ ex - (A) (B) (C)_
![image](https://github.com/Ninky0/classRegistration/assets/113659622/d6ffd9a2-7c95-44f1-ba2e-1c4fea9a15d4)

학생을 생성한다. (학생 이름) - 10명
_ex - (이은아) (남인경) (김태희) (도경수) (변백현) (조인성) (장효진) (김수현) (김아영) (홍재이)_
![image](https://github.com/Ninky0/classRegistration/assets/113659622/ceec367c-47d6-4548-bb8f-e66eecd0b184)
+) 예외 처리 : 이름 중복 방지
![image](https://github.com/Ninky0/classRegistration/assets/113659622/81cedaa2-2a6e-4b30-bc30-7c2c8f724fa5)

강의실, 교수, 학생 객체 생성이 정상적으로 작동하는 것을 확인할 수 있음. 교수의 강의 생성작업:
_ex - (A교수 객체지향언어 혜화관1호 수요일 1,2,3교시)
(B교수 운영체제 명진관2호 금요일 4,5,6교시)
(C교수 자료구조 학림관1호 월요일 5,6,7교시)_
![image](https://github.com/Ninky0/classRegistration/assets/113659622/82ecb0d2-d2c1-40e6-a385-553f87feb837)

강의가 정상적으로 생성되는 것을 확인할 수 있음. 학생의 수강신청 및 정보 확인할 수 있음. (이은아 객체지향언어 A교수 수요일 1,2,3 교시 혜화관1호 )
_ex - (남인경 자료구조 C교수 월요일 5,6,7교시 학림관1호 )_
![image](https://github.com/Ninky0/classRegistration/assets/113659622/828869aa-7e64-4896-9ae8-7da09f0f226f)

+) 예외처리 : 시간표가 겹치는 경우 수강 신청이 불가능함.
![image](https://github.com/Ninky0/classRegistration/assets/113659622/85a641a8-a1d7-423e-9018-b4882b2db8df)

학생의 수강 신청 취소 작업
![image](https://github.com/Ninky0/classRegistration/assets/113659622/38e59e98-ef5c-4bde-883a-dbd57df63655)

학생 수강 신청 완료 후 교수의 수강생 정보 확인
![image](https://github.com/Ninky0/classRegistration/assets/113659622/ed41576d-3cb9-4b98-b8ff-0cf56b15e216)

강의실 정보 확인
![image](https://github.com/Ninky0/classRegistration/assets/113659622/f9a29a53-6269-46bc-aed9-7b08c6e685a1)

교수의 강의 폐강 작업
![image](https://github.com/Ninky0/classRegistration/assets/113659622/3bb39866-4379-491a-bc01-a3fbcff5cbb7)
강의가 정상적으로 폐강된 것을 확인할 수 있음.

강의가 폐강되면 
-> 해당 강의를 신청한 학생과 해당 강의를 배정받은 강의실 객체에서도 강의 정보가 제거
![image](https://github.com/Ninky0/classRegistration/assets/113659622/bfa9f12c-93b5-44e5-a1a2-07ebc26fe2e2)
![image](https://github.com/Ninky0/classRegistration/assets/113659622/08fc9fc6-590c-4cd9-b462-408320cc56c9)

# 실행 종료후 DB확인
강의DB(LectureList.csv)
![image](https://github.com/Ninky0/classRegistration/assets/113659622/66b47e63-f6b2-41c6-93ba-ab7f900dc635)

강의실DB(ClassroomList.csv)
![image](https://github.com/Ninky0/classRegistration/assets/113659622/2099d6bb-196f-4abf-a414-6201b6994b26)

교수DB(ProfessorList.csv)
![image](https://github.com/Ninky0/classRegistration/assets/113659622/38772542-8c94-453c-94f7-2a8618f29381)

학생DB(StudentList.csv)
![image](https://github.com/Ninky0/classRegistration/assets/113659622/7bf5e269-ed30-4e9e-879f-a2844d1478fe)

