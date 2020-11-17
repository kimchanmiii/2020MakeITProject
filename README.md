# MakeITProject
안드로이드 스튜디오를 사용한 스타트업 팀 빌딩 혹은 프로젝트를 같이 진행하고자 하는 팀원을 구할 수 있는 플랫폼을 제공해주는 '팀 매칭' 서비스 입니다. 

## 목차

1. 서비스 소개
2. 팀 정보
3. 버전 및 실행환경
4. 주요 기능
5. 특이사항

<br>

## 1. 서비스 소개

<b>makeIT </b> 서비스는 스타트업 팀 빌딩 뿐만 아니라, 프로젝트를 같이 진행하고자 하는 팀 또는 팀원들을 구할 수 있는 '팀 빌딩' 플랫폼입니다. 

코로나로 인해 비대면 교육이 활성화되면서, 팀 프로젝트 인원을 구하는 것이 생각보다 어려움을 인지하였습니다.  '에브리타임' 같은 커뮤니티를 통해서 팀을 구하는 것도 가능하지만, '팀 빌딩' 플랫폼을 사용한다면 팀빌딩이 조금 더 수월할 것이라는 기대감이 생기게 되었습니다. 

따라서 <b>makeIT</b> 팀 빌딩 플랫폼을 기획하게 되었고, 아래와 같은 목적성을 가진 프로젝트를 진행하게 되었습니다.

- 초기 스타트업 팀원을 구성할 수 있다.
- 프로젝트를 진행할 팀/팀원을 구할 수 있다.
- 기업(스타트업)이 아니어도, 개인이 프로젝트를 진행할 팀원을 구할 수 있다.
- 자신의 프로필(이력서) 관리가 가능하다.
- 서로 원하는 조건에 충족하는 사람을 쉽고 빠르게 찾을 수 있다.

<b>makeIT</b> 는 '만든다' 라는 의미를 가지고 있지만, '해낸다' 라는 뜻도 가지고 있습니다. 어플명 <b>makeIT</b> 는 팀을 구상하고, 프로젝트를 성공적으로 수행하고자 하는 의미에서 부여하였습니다. 

<br>

## 2. 팀 정보

| 이름   | 소속       | 역할                              | github                         |
| ------ | ---------- | --------------------------------- | ------------------------------ |
| 김지홍 | 국민대학교 | UI 구성 및 로그인 기능 개발       | https://github.com/kimjihong9  |
| 김찬미 | 국민대학교 | 프론트엔드 개발 및 세션 기능 개발 | https://github.com/kimchanmiii |
| 윤서영 | 국민대학교 | Firebase 연동 및 백엔드 개발      | https://github.com/young43     |

<br>

## 3. 버전 및 실행환경

- 개발 환경

  - Language: Java
  - IDE: Android Studio

- 실행 환경

  - AVD: Android Q(10.0 x86_64)
  - minSDKVersion: 16
  - compileSDKVersion: 30
  
<br>

## 4. 주요 기능

### 계정 관리

- 로그인을 하지 않았던 상태라면, 초기화면에 로그인과 회원가입 화면이 표시됩니다. 
- 계정이 존재하면 로그인할 수 있고, 없다면 회원가입을 진행할 수 있습니다.
- 한번 로그인하면 세션이 유지되어 자동으로 로그인이 됩니다.
- 로그인 후 [MY] 탭에서 '로그아웃' 버튼 클릭시, 로그아웃이 가능합니다.

<img src="https://github.com/young43/makeITProject/blob/main/img/login_join.jpg?raw=true" alt="두번째 화면" width=500/>

### 이력서

- 각 회원들은 자신들의 이력서를 등록하고 관리할 수 있습니다. 
- 이름, 이메일, 연락처, 자기소개, 경력을 입력하고 이력서 등록이 가능합니다.  
- 경력은 최대 3개까지 입력할 수 있으며, 입사/퇴사 날짜를 입력할 수 있습니다. 
- 이력서를 등록하면 Firebase DB에 내용이 저장되고, 다시 이력서를 등록하려고 하면 이전에 저장했던 내용을 불러오게 됩니다.

<img src="https://github.com/young43/makeITProject/blob/main/img/resume.jpg?raw=true" alt="두번째 화면" width=500/>

### 찜(Bookmark)

- 로그인 후 [공고] 탭을 클릭하게 되면, 현재 등록된 프로젝트 목록을 볼 수 있으며, 마음에 드는 프로젝트는 '하트' 버튼을 통해 찜할 수 있습니다.
- [HOME] 탭에서 '찜 목록' 버튼을 누르면 찜해놨던 프로젝트 리스트를 볼 수 있습니다.
- 찜 목록에서 삭제를 원하면 다시 '하트' 버튼을 클릭하면 됩니다. 

<img src="https://github.com/young43/makeITProject/blob/main/img/bookmark.jpg?raw=true" alt="두번째 화면" width=500/>

### 프로젝트 관리

- 프로젝트 등록 및 조회
  - 모든 회원들은 프로젝트를 등록할 수 있으며, 프로젝트 삭제 권한은 등록한 회원에게 있습니다.
  - 제목, 지역, 인원, 내용, 담당 연락처 내용들을 입력하고 프로젝트 등록이 가능합니다. 
  - 등록한 프로젝트는 [공고] 탭에서 확인 가능하며, 프로젝트 제목 및 내용으로 검색이 가능합니다. 
  
<img src="https://github.com/young43/makeITProject/blob/main/img/project_show.jpg?raw=true" alt="두번째 화면" width=500/>
  
- 프로젝트 지원
  - 프로젝트 목록을 클릭하게 되면, 관련 프로젝트 정보가 화면에 표시됩니다.
  - 관심이 있는 프로젝트에 지원가능하며, 지원할 경우 이메일로 연동되어 자신의 이력서를 자동으로 불러오게 됩니다. 
  - [HOME] 탭 '진행 중인 프로젝트'에서 본인이 지원한 프로젝트를 확인할 수 있습니다.
  - 해당 프로젝트를 롱 클릭 시  삭제가 가능합니다. 
 
<img src="https://github.com/young43/makeITProject/blob/main/img/project_resume.jpg?raw=true" alt="두번째 화면" width=500/>

## 각자 맡은 부분 


### MainActivity
로그인 여부에 따라 보여지는 첫 화면을 결정하는 Activity이다. 로그인에 성공하여 앱이 실행되었을 때, 홈 화면을 띄운다. 화면 밑에 세가지 아이콘을 넣어 각 아이콘을 클릭했을 때 화면 간에 전환을 할 수 있도록 해주었다. 화면은 총 3개로 홈, 공고, 마이페이지로 구성되어있다. 각 화면간의 전환은 Fragment로 해주었다. 

```java
package kr.ac.kookmin.makeit;

import android.content.Intent;
import android.os.Bundle;
import android.view.MenuItem;

import androidx.appcompat.app.AppCompatActivity;
import androidx.fragment.app.Fragment;
import androidx.fragment.app.FragmentManager;
import androidx.fragment.app.FragmentTransaction;

import com.google.android.material.bottomnavigation.BottomNavigationView;
import com.google.firebase.firestore.FirebaseFirestore;


/**
 * @file MainActivity
 * @desc 로그인 여부에 따라 보여지는 첫 화면을 결정하는 Activity
 * @auther 김찬미(20191574)
 * @date 2020-11-01
 */

public class MainActivity extends AppCompatActivity {

    // 파이어베이스 연동
    public static FirebaseFirestore db = FirebaseFirestore.getInstance();

    private BottomNavigationView bottomNavigationView;

    private FragmentManager fm;
    private FragmentTransaction ft;

    private Fragment frag1;
    private Fragment frag2;
    private Fragment frag3;


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);


        // 기존에 로그인된 정보가 없으면 Login화면으로 이동
        if(SaveSharedPreference.getUserName(this).length() == 0) {
            Intent intent = new Intent(this, LoginActivity.class);
            startActivity(intent);
            finish();
        }

        // bottomNavigaion View를 id를 통해서 가져옴
        bottomNavigationView = findViewById(R.id.bottomNavi);

        // 무슨 아이콘을 선택했냐에 따라서 보여주는 화면(Fragment)전환이 이루어짐.
        // setOnNavigationItemSelectedListener 이벤트 설정
        bottomNavigationView.setOnNavigationItemSelectedListener(new BottomNavigationView.OnNavigationItemSelectedListener() {

            @Override
            public boolean onNavigationItemSelected(MenuItem menuItem) {
                switch (menuItem.getItemId()) {
                    case R.id.action_main:
                        setFrag(0, null);
                        break;
                    case R.id.action_notice:
                        setFrag(1,null);
                        break;
                    case R.id.action_mypage:
                        setFrag(2, null);
                        break;
                }
                return true;
            }
        });

        frag1 = new FragmentHome();
        frag2 = new FragmentNotice();
        frag3 = new FragmentMypage();

        // 첫 화면은 FragmentHome으로 설정.
        // setFrag에 주는 정수에 따라서 프래그먼트 트랜지션이 이루어짐.
        setFrag(0, null); // 첫 프래그먼트 화면 지정
    }

    public void setFrag(int n, Fragment frag) {
        fm = getSupportFragmentManager();
        ft = fm.beginTransaction();

        frag1 = new FragmentHome();
        frag2 = new FragmentNotice();
        frag3 = new FragmentMypage();

        switch (n) {
            case 0: // 메인
                if(frag != null)
                    frag1 = frag;

                bottomNavigationView.getMenu().findItem(R.id.action_main).setChecked(true);
                ft.replace(R.id.Main_Frame, frag1);
                ft.commit();
                break;

            case 1: // 공고
                if(frag != null)
                    frag2 = frag;

                bottomNavigationView.getMenu().findItem(R.id.action_notice).setChecked(true);
                ft.replace(R.id.Main_Frame, frag2);
                ft.commit();
                break;

            case 2: // 마이페이지
                if(frag != null)
                    frag3 = frag;

                bottomNavigationView.getMenu().findItem(R.id.action_mypage).setChecked(true);
                ft.replace(R.id.Main_Frame, frag3);
                ft.commit();
                break;

        }
    }
}
```

### FragmentHome
회원정보와 이력서 등록 및 보기, 찜했던 프로젝트 목록, 내가 진행 중인 프로젝트 목록을 모두 확인할 수 있는 Fragment이다. 저장되어 있는 모든 정보들을 각 기능에 맞게 보여주도록 구현하였다.
```java
package kr.ac.kookmin.makeit;

import android.content.Intent;
import android.os.Bundle;
import android.util.Log;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Button;
import android.widget.ListView;
import android.widget.TextView;

import androidx.annotation.NonNull;
import androidx.fragment.app.Fragment;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.firestore.DocumentReference;
import com.google.firebase.firestore.DocumentSnapshot;

import java.util.ArrayList;
import java.util.HashMap;

import static kr.ac.kookmin.makeit.MainActivity.db;

/**
 * @file FragmentHome
 * @desc 회원정보 및 찜버튼, 지원프로젝트 목록을 볼 수 있는 화면(프래그먼트)
 * @auther 김지홍(20191572), 김찬미(20191574)
 * @date 2020-11-01
 */
public class FragmentHome extends Fragment {

    // TODO: Rename parameter arguments, choose names that match
    // the fragment initialization parameters, e.g. ARG_ITEM_NUMBER
    private static final String ARG_PARAM1 = "param1";
    private static final String ARG_PARAM2 = "param2";

    // TODO: Rename and change types of parameters
    private String mParam1;
    private String mParam2;


    //////진행중인 프로젝트 목록 보여주기
    private ArrayList<ListItemProject> arrayData = new ArrayList<>();
    private ListViewProjectAdapter adapter;
    ListView listView;


    public FragmentHome() {
        // Required empty public constructor
    }


    // TODO: Rename and change types and number of parameters
    public static FragmentHome newInstance(String param1, String param2) {
        FragmentHome fragment = new FragmentHome();
        Bundle args = new Bundle();
        args.putString(ARG_PARAM1, param1);
        args.putString(ARG_PARAM2, param2);
        fragment.setArguments(args);
        return fragment;
    }

    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        if (getArguments() != null) {
            mParam1 = getArguments().getString(ARG_PARAM1);
            mParam2 = getArguments().getString(ARG_PARAM2);
        }
    }

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        final ViewGroup rootView = (ViewGroup) inflater.inflate(R.layout.fragment_home, container, false);

        // 현재 로그인된 ID로 표시
        String userId = SaveSharedPreference.getUserName(getContext());
        TextView textUser = (TextView) rootView.findViewById(R.id.text_username);
        textUser.setText(userId);

        // 찜 목록 리스트 보여주기(클릭 이벤트 추가)
        Button btnBookmark = (Button) rootView.findViewById(R.id.btn_bookmark_list);
        btnBookmark.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // 찜목록 액티비티로 전환
                Intent intent = new Intent(getContext(), BookmarkActivity.class);
                startActivity(intent);
            }
        });

        //이력서 등록화면으로 전환하기
        Button btnResume = (Button) rootView.findViewById(R.id.btn_resume);
        btnResume.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent(getContext(), ResumeActivity.class);
                startActivity(intent);
            }
        });

        //////진행중인 프로젝트 목록 보여주기
        adapter = new ListViewProjectAdapter(getContext(), android.R.layout.simple_list_item_multiple_choice, this);
        listView = (ListView) rootView.findViewById(R.id.list_myproject);
        listView.setAdapter(adapter);

        selectApplyOnFirebase();
        return rootView;
    }

    /////////
    public interface MyDataCallback{
        void onCallback();
    }

    public void selectApplyOnFirebase(){
        String id = SaveSharedPreference.getUserName(getContext());
        final DocumentReference docRef = db.collection("apply").document(id);
        docRef.get().addOnCompleteListener(new OnCompleteListener<DocumentSnapshot>() {
            @Override
            public void onComplete(@NonNull Task<DocumentSnapshot> task) {
                if (task.isSuccessful()) {
                    DocumentSnapshot document = task.getResult();
                    arrayData.clear();

                    if (document.exists()) {
                        ApplyInfo apply = new ApplyInfo((HashMap) document.getData());
                        HashMap<String, Boolean> projectMap = apply.getProjectMap();

                        for (String key : projectMap.keySet()) {
                            // 파이어베이스는 NoSQL이라 join을 지원하지 않음. 따라서 두번 쿼리실행.
                            selectProjectlistOnFirebase(key, new MyDataCallback() {
                                @Override
                                public void onCallback() {  // 데이터 로드 후에 화면에 표시
                                    // ListView update
                                    adapter.clear();
                                    adapter.setAll(arrayData);
                                    updateListView();
                                }
                            });
                        }
                    }

                } else {
                    Log.d("apply", "get failed with ", task.getException());
                }
            }
        });

    }

    public void selectProjectlistOnFirebase(String key, final MyDataCallback callback){
        db.collection("project_list").document(key)
            .get()
            .addOnCompleteListener(new OnCompleteListener<DocumentSnapshot>() {
                @Override
                public void onComplete(@NonNull Task<DocumentSnapshot> task) {
                    if(task.isSuccessful()) {
                        DocumentSnapshot document = task.getResult();
                        ListItemProject item = new ListItemProject((HashMap)document.getData());
                        item.setProject_id(document.getId());
                        // item.setSelected(true);

                        arrayData.add(item);
                        // Toast.makeText(BookmarkActivity.this, item.getTitle(), Toast.LENGTH_SHORT).show();
                    }

                    callback.onCallback();
                }
            });
    }


    public void updateListView(){
        adapter.notifyDataSetChanged();
        listView.setAdapter(adapter);
    }
}
```

### FragmentMypage
로그아웃 버튼이 존재하는 Fragment이다. '로그아웃'버튼을 누르면 로그인 키를 해제하여 현재 로그인되어있는 화면(Main)을 닫고, 로그인 및 회원가입을 할 수 있는 로그인 액티비티로 이동한다. 
```java
package kr.ac.kookmin.makeit;

import android.content.Intent;
import android.os.Bundle;
import android.view.LayoutInflater;
import android.view.View;
import android.view.ViewGroup;
import android.widget.Button;

import androidx.fragment.app.Fragment;

/**
 * @file FragmentMypage
 * @desc 로그아웃 버튼이 존재하는 화면(프래그먼트)
 * @auther 김찬미(20191574)
 * @date 2020-11-01
 */
public class FragmentMypage extends Fragment {

    // TODO: Rename parameter arguments, choose names that match
    // the fragment initialization parameters, e.g. ARG_ITEM_NUMBER
    private static final String ARG_PARAM1 = "param1";
    private static final String ARG_PARAM2 = "param2";

    // TODO: Rename and change types of parameters
    private String mParam1;
    private String mParam2;

    public FragmentMypage() {
        // Required empty public constructor
    }

    /**
     * Use this factory method to create a new instance of
     * this fragment using the provided parameters.
     *
     * @param param1 Parameter 1.
     * @param param2 Parameter 2.
     * @return A new instance of fragment FragmentMypage.
     */
    // TODO: Rename and change types and number of parameters
    public static FragmentMypage newInstance(String param1, String param2) {
        FragmentMypage fragment = new FragmentMypage();
        Bundle args = new Bundle();
        args.putString(ARG_PARAM1, param1);
        args.putString(ARG_PARAM2, param2);
        fragment.setArguments(args);
        return fragment;
    }

    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        if (getArguments() != null) {
            mParam1 = getArguments().getString(ARG_PARAM1);
            mParam2 = getArguments().getString(ARG_PARAM2);
        }
    }

    @Override
    public View onCreateView(LayoutInflater inflater, ViewGroup container,
                             Bundle savedInstanceState) {
        // Inflate the layout for this fragment
        final ViewGroup rootView = (ViewGroup) inflater.inflate(R.layout.fragment_mypage, container, false);

        // 로그아웃 기능 구현
        Button btnLogout = (Button) rootView.findViewById(R.id.btn_logout);
        btnLogout.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                // 로그인 key 해제
                SaveSharedPreference.setUserName(getContext(), "");

                // 현재 액티비티(Main) 닫고, 로그인 액티비티로 이동
                Intent intent = new Intent(getContext(), LoginActivity.class);
                startActivity(intent);
                getActivity().finish();
            }
        });

        return rootView;
    }
}
```

### SavedSharedPreference 
자동 로그인 및 로그인 유지를 위한 클래스이다. 한번 로그인했던 기록이 있다면 계정 정보를 저장하고 저장된 정보를 가져와 앱을 껐다가 다시 실행시켰을 때에도 정보가 저장되게끔 만들어주었다. 로그아웃 기능도 구현되어있다. 
```java
package kr.ac.kookmin.makeit;


import android.content.Context;
import android.content.SharedPreferences;
import android.preference.PreferenceManager;

/**
 * @file SaveSharedPreference
 * @desc 자동 로그인 및 로그인 유지를 위한 클래스
 * @auther 김지홍(20191572), 김찬미(20191574)
 * @date 2020-11-02
 */
public class SaveSharedPreference {
    static final String PREF_USER_NAME = "username";

    static SharedPreferences getSharedPreferences(Context ctx) {
        return PreferenceManager.getDefaultSharedPreferences(ctx);
    }

    // 계정 정보 저장
    public static void setUserName(Context ctx, String userName) {
        SharedPreferences.Editor editor = getSharedPreferences(ctx).edit();
        editor.putString(PREF_USER_NAME, userName);
        editor.commit();
    }

    // 저장된 정보 가져오기
    public static String getUserName(Context ctx) {
        return getSharedPreferences(ctx).getString(PREF_USER_NAME, "");
    }

    // 로그아웃
    public static void clearUserName(Context ctx) {
        SharedPreferences.Editor editor = getSharedPreferences(ctx).edit();
        editor.clear();
        editor.commit();
    }

}

```

### ProjectInfoActivity
각 프로젝트가 클릭되었을 때 보여지는 프로젝트 info화면이다. 화면은 ScrollView로 설정해주었으며 저장된 제목, 지역, 구하는 인원 수, 구인 내용, 담당자 연락처와 이메일을 보여주도록 설정하였다. 지원하고 싶은 프로젝트가 생겼을 때 '프로젝트 지원'버튼을 누르면 자신이 작성했던 이력서가 담당자 이메일로 보내지게끔 설정하였다. 
```java
package kr.ac.kookmin.makeit;

import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.text.method.ScrollingMovementMethod;
import android.util.Log;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Spinner;
import android.widget.TextView;
import android.widget.Toast;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.OnFailureListener;
import com.google.android.gms.tasks.OnSuccessListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.firestore.DocumentSnapshot;
import com.google.firebase.firestore.SetOptions;

import java.util.HashMap;
import java.util.Map;

import static kr.ac.kookmin.makeit.MainActivity.db;

/**
 * @file ProjectInfoActivity
 * @desc 각 프로젝트가 클릭되었을 때 보여지는 프로젝트 info 화면(Activity)
 * @auther 김찬미(20191574), 윤서영(20191633)
 * @date 2020-11-01
 */

public class ProjectInfoActivity extends AppCompatActivity {

    HashMap<String, Object> data;
    TextView textTitle, textContent, textPhone, textEmail, textRegion, textMember, textDate;

    public interface MyDataCallback {
        void onCallback(boolean exists, ResumeInfo info);
    }

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_project_info);


        Intent intent = getIntent();
        data = (HashMap) intent.getSerializableExtra("projectInfo");

        // TextView 데이터 매칭
        textTitle = (TextView) findViewById(R.id.text_project_title);
        textContent = (TextView) findViewById(R.id.text_project_content);
        textPhone = (TextView) findViewById(R.id.text_project_phone);
        textEmail = (TextView) findViewById(R.id.text_project_email);
        textRegion = (TextView) findViewById(R.id.text_project_region);
        textMember = (TextView) findViewById(R.id.text_project_member);
        textDate = (TextView) findViewById(R.id.text_project_date);

        textTitle.setText((String)data.get("title"));
        textContent.setText((String)data.get("content"));
        textPhone.setText((String)data.get("phonenumber"));
        textEmail.setText((String)data.get("email"));
        textRegion.setText((String)data.get("region"));
        textMember.setText(String.valueOf(data.get("person")));  // person은 number형(=long)형이다.
        textDate.setText((String)data.get("upload_date"));

        // 스크롤 가능하게 설정
        textContent.setMovementMethod(new ScrollingMovementMethod());

        // 프로젝트 지원 버튼 이벤트 설정
        // 자신의 이력서 내용을 바탕으로 이메일 작성
        Button btnJoin = (Button) findViewById(R.id.btn_join_project);
        btnJoin.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {


                // 이력서 내용 조회
                selectQueryOnFirebase(new MyDataCallback() {
                    @Override
                    public void onCallback(boolean exists, ResumeInfo info) {
                        // 메일 관련 내용
                        String receiver = (String)data.get("email");
                        String title = (String)data.get("title") + " 지원합니다.";
                        String resume = "";

                        if(exists){
                            resume += "이름: " + info.getResume_name() + "\n"
                                    + "이메일: " + info.getResume_email() + "\n"
                                    + "연락처: " + info.getResume_phone() + "\n\n"
                                    + "[자기소개]" + "\n"
                                    + info.getResume_introduction() + "\n\n";

                            if(info.getResume_company1().length() > 0){
                                resume += "[경력1]" + "\n"
                                        + info.getResume_company1() + ") " + info.getResume_company_date1() + "\n\n";
                            }

                            if(info.getResume_company2().length() > 0){
                                resume += "[경력2]" + "\n"
                                        + info.getResume_company2() + ") " + info.getResume_company_date2() + "\n\n";
                            }

                            if(info.getResume_company3().length() > 0){
                                resume += "[경력3]" + "\n"
                                        + info.getResume_company3() + ") " + info.getResume_company_date3() + "\n\n";
                            }
                        }


                        // Firebase 지원 collection 데이터 추가
                        String id = SaveSharedPreference.getUserName(ProjectInfoActivity.this);  // 현재 로그인된 id 가져옴
                        String project_id = (String)data.get("project_id");
                        Map<String, Object> apply = new HashMap<>();
                        apply.put("id", id);
                        apply.put(project_id, true);

                        // 찜 목록 데이터 업데이트
                        db.collection("apply").document(id)
                            .set(apply, SetOptions.merge())  // merge옵션으로 update 및 추가 가능
                            .addOnSuccessListener(new OnSuccessListener<Void>() {
                                @Override
                                public void onSuccess(Void aVoid) {
                                    Log.e("apply", "Success update data on firebase");
                                }
                            })
                            .addOnFailureListener(new OnFailureListener() {
                                @Override
                                public void onFailure(@NonNull Exception e) {
                                    Log.w("apply", "Error update data", e);
                                }
                            });

                        Intent email = new Intent(Intent.ACTION_SEND);
                        email.setType("plain/Text");
                        email.putExtra(Intent.EXTRA_EMAIL, new String[] { receiver });     // 받는사람 설정
                        email.putExtra(Intent.EXTRA_SUBJECT, title);
                        email.putExtra(Intent.EXTRA_TEXT, resume);
                        email.setType("message/rfc822");
                        startActivity(email);

                    }
                });



            }
        });

    }

    public void selectQueryOnFirebase(final MyDataCallback callback){
        // Firebase 연동
        // 프로젝트 리스트를 긁어서 보여준다.
        // Collection(=DB) -> Document(=row)으로 구성되어있으며, column은 getData로 Map형태로 가져올 수 있다.
        String id = SaveSharedPreference.getUserName(ProjectInfoActivity.this);

        db.collection("resume").document(id)
                .get()
                .addOnCompleteListener(new OnCompleteListener<DocumentSnapshot>() {
                    @Override
                    public void onComplete(@NonNull Task<DocumentSnapshot> task) {
                        if(task.isSuccessful()) {
                            DocumentSnapshot document = task.getResult();
                            if(document.getData() != null){
                                ResumeInfo info = new ResumeInfo((HashMap) document.getData());
                                callback.onCallback(true, info);
                            }else{
                                callback.onCallback(false, null);
                            }

                        }else{
                            callback.onCallback(false, null);
                        }

                    }
                })
                .addOnFailureListener(new OnFailureListener() {
                    @Override
                    public void onFailure(@NonNull Exception e) {
                        callback.onCallback(false, null);
                    }
                });
    }
}
```

### ResumeInfo
이력서 관련 클래스로 이력서에 들어가는 정보들을 모두 저장한다. 

```java
package kr.ac.kookmin.makeit;

import java.util.HashMap;
import java.util.Map;

/**
 * @file ResumeInfo
 * @desc 이력서 관련 클래스
 * @auther 김찬미(20191574)
 * @date 2020-11-12
 */

public class ResumeInfo {
    private String resume_id;
    private String resume_name;
    private String resume_email;
    private String resume_phone;
    private String resume_introduction;
    private String resume_company1;
    private String resume_company2;
    private String resume_company3;
    private String resume_company_date1;
    private String resume_company_date2;
    private String resume_company_date3;



    public ResumeInfo(){ }

    public ResumeInfo(String resume_id, String resume_name, String resume_email, String resume_phone,
                      String resume_introduction, String resume_company1, String resume_company2, String resume_company3,
                        String resume_company_date1, String resume_company_date2, String resume_company_date3){
        this.resume_id = resume_id;
        this.resume_name = resume_name;
        this.resume_email = resume_email;
        this.resume_phone = resume_phone;
        this.resume_introduction = resume_introduction;
        this.resume_company1 = resume_company1;
        this.resume_company2 = resume_company2;
        this.resume_company3 = resume_company3;
        this.resume_company_date1 = resume_company_date1;
        this.resume_company_date2 = resume_company_date2;
        this.resume_company_date3 = resume_company_date3;
    }

    public ResumeInfo(HashMap<String, Object> map){
        this.resume_id = (String) map.get("resume_id");
        this.resume_name = (String) map.get("resume_name");
        this.resume_email = (String) map.get("resume_email");
        this.resume_phone = (String) map.get("resume_phone");
        this.resume_introduction = (String) map.get("resume_introduction");
        this.resume_company1 = (String) map.get("resume_company1");
        this.resume_company2 = (String) map.get("resume_company2");
        this.resume_company3 = (String) map.get("resume_company3");
        this.resume_company_date1 = (String) map.get("resume_company_date1");
        this.resume_company_date2 = (String) map.get("resume_company_date2");
        this.resume_company_date3 = (String) map.get("resume_company_date3");
    }

    public Map<String, Object> toMap(){
        HashMap<String, Object> map = new HashMap<>();
        map.put("resume_id", resume_id);
        map.put("resume_name", resume_name);
        map.put("resume_email", resume_email);
        map.put("resume_phone", resume_phone);
        map.put("resume_introduction", resume_introduction);
        map.put("resume_company1", resume_company1);
        map.put("resume_company2", resume_company2);
        map.put("resume_company3", resume_company3);
        map.put("resume_company_date1", resume_company_date1);
        map.put("resume_company_date2", resume_company_date2);
        map.put("resume_company_date3", resume_company_date3);

        return map;
    }


    public String getResume_id() { return resume_id; }

    public void setResume_id(String resume_id) { this.resume_id = resume_id; }

    public String getResume_name() { return resume_name; }

    public void setResume_name(String resume_name) { this.resume_name = resume_name; }

    public String getResume_email() { return resume_email; }

    public void setResume_email(String resume_email) { this.resume_email = resume_email; }

    public String getResume_phone() { return resume_phone; }

    public void setResume_phone(String resume_phone) { this.resume_phone = resume_phone; }

    public String getResume_introduction() { return resume_introduction; }

    public void setResume_introduction(String resume_introduction) { this.resume_introduction = resume_introduction; }

    public String getResume_company1() { return resume_company1; }

    public void setResume_company1(String resume_company1) { this.resume_company1 = resume_company1; }

    public String getResume_company2() { return resume_company2; }

    public void setResume_company2(String resume_company2) { this.resume_company2 = resume_company2; }

    public String getResume_company3() { return resume_company3; }

    public void setResume_company3(String resume_company3) { this.resume_company3 = resume_company3; }

    public String getResume_company_date1() { return resume_company_date1; }

    public void setResume_company_date1(String resume_company_date1) { this.resume_company_date1 = resume_company_date1; }

    public String getResume_company_date2() { return resume_company_date2; }

    public void setResume_company_date2(String resume_company_date2) { this.resume_company_date2 = resume_company_date2; }

    public String getResume_company_date3() { return resume_company_date3; }

    public void setResume_company_date3(String resume_company_date3) { this.resume_company_date3 = resume_company_date3; }
}
```
### ResumeActivity
이력서를 등록하기 위한 Activity이다. 홈 화면에서 '이력서' 버튼을 누르면 이력서를 등록할 수 있는 화면으로 전환된다. 이력서 등록 화면에서 정보 입력에 필요한 이름, 이메일, 연락처, 자기소개, 경력을 모두 editText로 받아와 저장한다. 입력을 모두 완료한 뒤 '이력서 등록' 버튼을 누르면 입력된 정보를 바탕으로 이력서가 등록된다. 이 정보들은 모두 Firebase에 저장했으며 어플을 꺼도 정보는 저장된다. 각 함수의 사용 이유에 대해선 주석에 설명해 놓았다. 
```java 
package kr.ac.kookmin.makeit;

import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.util.Log;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.OnFailureListener;
import com.google.android.gms.tasks.OnSuccessListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.firestore.CollectionReference;
import com.google.firebase.firestore.DocumentReference;
import com.google.firebase.firestore.DocumentSnapshot;
import com.google.firebase.firestore.Query;
import com.google.firebase.firestore.QueryDocumentSnapshot;
import com.google.firebase.firestore.QuerySnapshot;
import com.google.firebase.firestore.SetOptions;

import java.util.HashMap;

import static kr.ac.kookmin.makeit.MainActivity.db;

/**
 * @file ResumeActivity
 * @desc 이력서를 등록하기 위한 Activity
 * @auther 김찬미(20191574)
 * @date 2020-11-12
 */

public class ResumeActivity extends AppCompatActivity {

    EditText editName, editEmail, editPhone, editIntroduction, editCompany1, editCompany2, editCompany3,
                editInYear1, editInYear2, editInYear3, editOutYear1, editOutYear2, editOutYear3,
                editInMonth1, editInMonth2, editInMonth3, editOutMonth1, editOutMonth2, editOutMonth3;


    public interface MyDataCallback {
        void onCallback(boolean exists, ResumeInfo info);
    }

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_resume);


        selectQueryOnFirebase(new MyDataCallback() {
            @Override
            public void onCallback(boolean exists, ResumeInfo info) {
                // 이력서에 대한 정보가 있으면 화면에 표시해줌.
                if(exists){
                    editName.setText(info.getResume_name());
                    editEmail.setText(info.getResume_email());
                    editPhone.setText(info.getResume_phone());
                    editIntroduction.setText(info.getResume_introduction());
                    editCompany1.setText(info.getResume_company1());
                    editCompany2.setText(info.getResume_company2());
                    editCompany3.setText(info.getResume_company3());

                    // 날짜형식: 201909/202010 -> 파싱필요
                    if(info.getResume_company_date1().length() > 1 && info.getResume_company_date1().split("/")[0].length() == 6){
                        String inyear1 = info.getResume_company_date1().split("/")[0].substring(0, 4);
                        String inmonth1 = info.getResume_company_date1().split("/")[0].substring(4, 6);

                        editInYear1.setText(inyear1);
                        editInMonth1.setText(inmonth1);
                    }

                    if(info.getResume_company_date2().length() > 2 && info.getResume_company_date2().split("/")[0].length() == 6){
                        String inyear2 = info.getResume_company_date2().split("/")[0].substring(0, 4);
                        String inmonth2 = info.getResume_company_date2().split("/")[0].substring(4, 6);

                        editInYear2.setText(inyear2);
                        editInMonth2.setText(inmonth2);
                    }

                    if(info.getResume_company_date3().length() > 2 && info.getResume_company_date3().split("/")[0].length() == 6){
                        String inyear3 = info.getResume_company_date3().split("/")[0].substring(0, 4);
                        String inmonth3 = info.getResume_company_date3().split("/")[0].substring(4, 6);

                        editInYear3.setText(inyear3);
                        editInMonth3.setText(inmonth3);
                    }

                    if(info.getResume_company_date1().length() > 2 && info.getResume_company_date1().split("/")[1].length() == 6){
                        String outyear1 = info.getResume_company_date1().split("/")[1].substring(0, 4);
                        String outmonth1 = info.getResume_company_date1().split("/")[1].substring(4, 6);

                        editOutYear1.setText(outyear1);
                        editOutMonth1.setText(outmonth1);
                    }

                    if(info.getResume_company_date2().length() > 2 && info.getResume_company_date2().split("/")[1].length() == 6){
                        String outyear2 = info.getResume_company_date2().split("/")[1].substring(0, 4);
                        String outmonth2 = info.getResume_company_date2().split("/")[1].substring(4, 6);

                        editOutYear2.setText(outyear2);
                        editOutMonth2.setText(outmonth2);
                    }

                    if(info.getResume_company_date3().length() > 2 && info.getResume_company_date3().split("/")[1].length() == 6){
                        String outyear3 = info.getResume_company_date3().split("/")[1].substring(0, 4);
                        String outmonth3 = info.getResume_company_date3().split("/")[1].substring(4, 6);

                        editOutYear3.setText(outyear3);
                        editOutMonth3.setText(outmonth3);
                    }


                }

                onRestart();
            }
        });


        //editText 매칭
        editName = (EditText) findViewById(R.id.edit_resume_name);
        editEmail = (EditText) findViewById(R.id.edit_resume_email);
        editPhone = (EditText) findViewById(R.id.edit_resume_phone);
        editIntroduction = (EditText) findViewById(R.id.edit_resume_introduction);
        editCompany1 = (EditText) findViewById(R.id.resume_company_name1);
        editCompany2 = (EditText) findViewById(R.id.resume_company_name2);
        editCompany3 = (EditText) findViewById(R.id.resume_company_name3);
        editInYear1 = (EditText) findViewById(R.id.resume_in_year1);
        editInYear2 = (EditText) findViewById(R.id.resume_in_year2);
        editInYear3 = (EditText) findViewById(R.id.resume_in_year3);
        editOutYear1 = (EditText) findViewById(R.id.resume_out_year1);
        editOutYear2 = (EditText) findViewById(R.id.resume_out_year2);
        editOutYear3 = (EditText) findViewById(R.id.resume_out_year3);
        editInMonth1 = (EditText) findViewById(R.id.resume_in_month1);
        editInMonth2 = (EditText) findViewById(R.id.resume_in_month2);
        editInMonth3 = (EditText) findViewById(R.id.resume_in_month3);
        editOutMonth1 = (EditText) findViewById(R.id.resume_out_month1);
        editOutMonth2 = (EditText) findViewById(R.id.resume_out_month2);
        editOutMonth3 = (EditText) findViewById(R.id.resume_out_month3);

        //이력서 등록 이벤트
        Button btnResume = (Button) findViewById(R.id.btn_register_resume);
        btnResume.setOnClickListener(new View.OnClickListener(){
            @Override
            public void onClick(View v) {
                String id = SaveSharedPreference.getUserName(ResumeActivity.this);  // 현재 로그인된 id 가져옴
                String name = editName.getText().toString().trim();
                String email = editEmail.getText().toString().trim();
                String phone = editPhone.getText().toString().trim();
                String introduction = editIntroduction.getText().toString().trim();
                String company1 = editCompany1.getText().toString().trim();
                String company2 = editCompany2.getText().toString().trim();
                String company3 = editCompany3.getText().toString().trim();
                String date1 = editInYear1.getText().toString() + editInMonth1.getText().toString() + "/" + editOutYear1.getText().toString() + editOutMonth1.getText().toString();
                String date2 = editInYear2.getText().toString() + editInMonth2.getText().toString() + "/" + editOutYear2.getText().toString() + editOutMonth2.getText().toString();
                String date3 = editInYear3.getText().toString() + editInMonth3.getText().toString() + "/" + editOutYear3.getText().toString() + editOutMonth3.getText().toString();

                // 날짜 유효성 체크
                if(date1.length() > 2 && !(date1.length() == 7 || date1.length() == 13)){
                    Toast.makeText(ResumeActivity.this, "날짜 입력 다시 확인해주세요.", Toast.LENGTH_SHORT).show();
                    return;
                }
                if(date2.length() > 2 && !(date2.length() == 7 || date2.length() == 13)){
                    Toast.makeText(ResumeActivity.this, "날짜 입력 다시 확인해주세요.", Toast.LENGTH_SHORT).show();
                    return;
                }
                if(date3.length() > 2 && !(date3.length() == 7 || date3.length() == 13)){
                    Toast.makeText(ResumeActivity.this, "날짜 입력 다시 확인해주세요.", Toast.LENGTH_SHORT).show();
                    return;
                }

                ResumeInfo resume = new ResumeInfo(id, name, email, phone, introduction, company1, company2, company3, date1, date2, date3);
                HashMap<String, Object> data = (HashMap)resume.toMap();

                // Firebase 연동 및 resume콜렉션 데이터 추가
                db.collection("resume").document(id)
                    .set(data, SetOptions.merge())  // merge옵션으로 update 및 추가 가능
                    .addOnSuccessListener(new OnSuccessListener<Void>() {
                        @Override
                        public void onSuccess(Void aVoid) {
                            Log.e("resume", "Success update data on firebase");
                            Toast.makeText(ResumeActivity.this, "정상적으로 등록되었습니다.", Toast.LENGTH_SHORT).show();
                            finish();
                        }
                    })
                    .addOnFailureListener(new OnFailureListener() {
                        @Override
                        public void onFailure(@NonNull Exception e) {
                            Log.w("resume", "Error update data", e);
                        }
                    });

            }
        });
    }


    public void selectQueryOnFirebase(final MyDataCallback callback){
        // Firebase 연동
        // 프로젝트 리스트를 긁어서 보여준다.
        // Collection(=DB) -> Document(=row)으로 구성되어있으며, column은 getData로 Map형태로 가져올 수 있다.
        String id = SaveSharedPreference.getUserName(ResumeActivity.this);

        db.collection("resume").document(id)
            .get()
            .addOnCompleteListener(new OnCompleteListener<DocumentSnapshot>() {
                @Override
                public void onComplete(@NonNull Task<DocumentSnapshot> task) {
                    if(task.isSuccessful()) {
                        DocumentSnapshot document = task.getResult();
                        if(document.getData() != null){
                            ResumeInfo info = new ResumeInfo((HashMap) document.getData());
                            callback.onCallback(true, info);
                        }else{
                            callback.onCallback(false, null);
                        }

                    }else{
                        callback.onCallback(false, null);
                    }

                }
            })
            .addOnFailureListener(new OnFailureListener() {
                @Override
                public void onFailure(@NonNull Exception e) {
                    callback.onCallback(false, null);
                }
            });
    }
}
```

