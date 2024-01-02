## Introduction
Welcome to the CodeKoro Code Documentation, your comprehensive guide to the architecture and functionalities of CodeKoro. CodeKoro comprises three essential modules: Frontend, Backend, and Compiler. Each module plays a crucial role in delivering a seamless and powerful coding experience.

### Frontend
![asset](https://qtecsolution.com/media/technologies/React_JS_1oFeSaJ.png)

- Technology: Built with React
- Description: The Frontend Module serves as the user interface, providing an interactive and intuitive platform for participants. Leveraging React, it ensures a responsive and dynamic experience, enabling users to navigate through contests, problems, and their personalized dashboards effortlessly.

### Backend
![asset](https://d1wrxu8gicsgam.cloudfront.net/wp-content/files/django-logo-big.jpg)

- Technology: Built with Django
- Description: The Backend Module serves as the backbone of CodeKoro, handling data storage, user authentication, and business logic. Powered by Django, it ensures a robust and scalable architecture, facilitating seamless communication between the Frontend and the Database. User profiles, contest data, and submissions are managed with efficiency.

### Compiler
![asset](https://miro.medium.com/v2/resize:fit:1400/1*ycIMlwgwicqlO6PcFRA-Iw.png)

- Technology: Built with Vanilla Python
- Description: The Compiler Module is the engine behind the execution of code submissions. Built with Vanilla Python, it ensures the secure and efficient compilation and execution of code, providing real-time feedback to users. This module is pivotal in assessing the correctness and efficiency of participants' solutions.

## Frontend
### Project Structure
        ├───AdminPage/
        │   ├───AddProblemToContest/
        │   │   ├───AddProblemToContest.tsx
        │   │   └───style.css
        │   ├───ContestPage/
        │   │   ├───ContestPage.tsx
        │   │   └───style.css
        │   ├───CreateContestPage/
        │   │   ├───CreateContestPage.tsx
        │   │   └───style.css
        │   ├───CreateProblemPage/
        │   │   ├───CreateProblemPage.tsx
        │   │   └───style.css
        │   ├───ProblemsPage/
        │   │   ├───ProblemPage.tsx
        │   │   └───style.css
        │   ├───StressTestPage/
        │   │   ├───StressTestPage.tsx
        │   │   └───style.css
        │   ├───AdminPage.tsx
        │   ├───Create
        │   └───style.css
        ├───AuthenticationPage/
        │   ├───AuthenticationPage.tsx
        │   ├───SignIn.tsx
        │   ├───SignUp.tsx
        │   └───style.css
        ├───ContestPage/
        │   ├───MySubmissions/
        │   │   ├───MySubmissions.tsx
        │   │   └───style.css
        │   ├───Problems.tsx/
        │   │   ├───components/
        │   │   │   └───InputOutput.tsx
        │   │   ├───problems.tsx
        │   │   └───style.css
        │   ├───Standings/
        │   │   ├───ProblemItem/
        │   │   │   ├───ProblemItem.tsx
        │   │   │   └───style.txt
        │   │   ├───ProblemNumberItem/
        │   │   │   ├───ProblemtNumberItem.tsx
        │   │   │   └───style.tsx
        │   │   ├───Standings.tsx
        │   │   └───style.css
        │   ├───SubmitPage.tsx/
        │   │   ├───SubmitPage.tsx
        │   │   └───style.css
        │   ├───components/
        │   │   ├───Contests.tsx
        │   │   ├───NavbarButtonCon.tsx
        │   │   ├───NavbarButtonText.tsx
        │   │   ├───NavbarCon.tsx
        │   │   ├───Stand.tsx
        │   │   ├───Submission.tsx
        │   │   └───style.css
        │   ├───ContestPage.tsx
        │   ├───ProblemsList.tsx
        │   └───style.css
        ├───HomePage/
        │   ├───ProblemSet/
        │   │   ├───ProSet.tsx
        │   │   ├───ProblemSet.tsx
        │   │   └───style.css
        │   ├───Ranking/
        │   │   ├───Rank.tsx
        │   │   ├───Ranking.tsx
        │   │   └───style.css
        │   ├───components/
        │   │   ├───Navbar.tsx
        │   │   ├───NavbarButton.tsx
        │   │   ├───OnlyContest.tsx
        │   │   ├───RecCont.tsx
        │   │   ├───RecentContest.tsx
        │   │   ├───UpCont.tsx
        │   │   ├───UpcommingContest.tsx
        │   │   └───style.css
        │   ├───HomePage.tsx
        │   └───style.css
        ├───Profilepage/
        │   ├───components/
        │   │   ├───NavbarProfile.tsx
        │   │   ├───NavbarProfileButton.tsx
        │   │   ├───SolvedDetails.tsx
        │   │   └───style.css
        │   ├───Profilepage.tsx
        │   └───style.css
        ├───assets/
        │   ├───logo.png
        │   └───react.svg
        ├───App.css
        ├───App.tsx
        ├───Utils.tsx
        ├───index.css
        ├───main.tsx
        └───vite-env.d.ts

### AdminPage

#### AddProblemToContest
``` Type
    <AddProblemToContest />
```

#### ProblemPage
``` Type
    <ProblemPage />
```

#### CreateContetPae
``` Type
    <CreateContest />
```

#### ContestPage
``` Type
    <CreateContest />
```

#### StressTestPage
``` Type
    <StressTestPage />
```

#### CreateProblem
``` Type
    <CreateProblem />
```

### HomePage

#### OnlyContestPage
##### UpcommingContest
``` Type
    <UpcommingContest />
```

##### RecentContest
``` Type
    <RecentContest />
```

##### RecentContest
``` Type
    <RecentContest />
```

#### Problemset
``` TypeScript
    <ProblemSet />
```

##### ProSet
``` TypeScript
    <ProSet problem_id={problem.problem_number} isActive={state.page == 1} name={problem.problem_name} solved={'🧑🏻 ' + problem.solve_count} /> 
```

#### Ranking
``` TypeScript
    <<Ranking/> />
```

##### Rank
``` TypeScript
    <Rank key={index} position={index + 1} name={r.fullname} contests={r.contest_attend} solved={r.problem_solve} />
```

### Contest Arena
#### ProblemList
``` TypeScript
    <ProblemList id={id + ""} pageChanger={detail}/>
```
#### Problems
``` TypeScript
    <Problems id={state.problemId} />
```

#### Submit
``` TypeScript
     <SubmitPage id={state.problemId + ""} contest={id + ""}/>
```

#### MySubmission
``` TypeScript
     <MySubmissions contest={id + ""}/>
```

#### Standing
``` TypeScript
     <Standigs contest={id + ""}/>
```

### Authentication
#### Sign in
``` TypeScript
     <SignIn />
```

#### Sign in
``` TypeScript
     <Sign Up/>
```

## Backend

### Project Sturcure

    ├───.idea/
    │   ├───inspectionProfiles/
    │   │   ├───Project_Default.xml
    │   │   └───profiles_settings.xml
    │   ├───.gitignore
    │   ├───.name
    │   ├───Backend.iml
    │   ├───misc.xml
    │   ├───modules.xml
    │   ├───vcs.xml
    │   └───workspace.xml
    ├───Backend/
    │   ├───.idea/
    │   │   ├───inspectionProfiles/
    │   │   │   ├───Project_Default.xml
    │   │   │   └───profiles_settings.xml
    │   │   ├───.gitignore
    │   │   ├───Backend.iml
    │   │   ├───misc.xml
    │   │   ├───modules.xml
    │   │   ├───vcs.xml
    │   │   └───workspace.xml
    │   ├───__pycache__/
    │   │   ├───__init__.cpython-310.pyc
    │   │   ├───__init__.cpython-311.pyc
    │   │   ├───settings.cpython-310.pyc
    │   │   ├───settings.cpython-311.pyc
    │   │   ├───urls.cpython-310.pyc
    │   │   ├───urls.cpython-311.pyc
    │   │   ├───wsgi.cpython-310.pyc
    │   │   └───wsgi.cpython-311.pyc
    │   ├───__init__.py
    │   ├───asgi.py
    │   ├───celery.py
    │   ├───settings.py
    │   ├───urls.py
    │   └───wsgi.py
    ├───CodeKoro/
    │   ├───__pycache__/
    │   │   ├───__init__.cpython-310.pyc
    │   │   ├───__init__.cpython-311.pyc
    │   │   ├───admin.cpython-310.pyc
    │   │   ├───admin.cpython-311.pyc
    │   │   ├───apps.cpython-310.pyc
    │   │   ├───apps.cpython-311.pyc
    │   │   ├───authenticate.cpython-310.pyc
    │   │   ├───models.cpython-310.pyc
    │   │   ├───models.cpython-311.pyc
    │   │   ├───serializers.cpython-310.pyc
    │   │   ├───urls.cpython-310.pyc
    │   │   ├───utils.cpython-310.pyc
    │   │   └───views.cpython-310.pyc
    │   ├───apis/
    │   │   ├───__pycache__/
    │   │   │   ├───contest.cpython-310.pyc
    │   │   │   ├───problem.cpython-310.pyc
    │   │   │   └───user.cpython-310.pyc
    │   │   ├───contest.py
    │   │   ├───problem.py
    │   │   └───user.py
    │   ├───migrations/
    │   │   ├───__pycache__/
    │   │   │   ├───0002_alter_country_table.cpython-310.pyc
    │   │   │   ├───0003_alter_country_table.cpython-310.pyc
    │   │   │   ├───0004_user.cpython-310.pyc
    │   │   │   ├───0005_alter_user_email_alter_user_username_and_more.cpython-310.pyc
    │   │   │   └───__init__.cpython-310.pyc
    │   │   ├───0001_initial.py
    │   │   ├───0002_languagemodel_submissionmodel_code_and_more.py
    │   │   ├───0003_verdict_submissionmodel_verdict_text_and_more.py
    │   │   ├───0004_rename_contest_id_submissionmodel_contest_and_more.py
    │   │   ├───0005_contestsubmissionmodel.py
    │   │   ├───0006_alter_contestsubmissionmodel_id.py
    │   │   ├───0007_alter_contestsubmissionmodel_unique_together.py
    │   │   ├───0008_contestsubmissionmodel_accepted_and_more.py
    │   │   ├───0009_penaltymodel.py
    │   │   ├───0010_rename_penaltymodel_penaltymodel_penalty.py
    │   │   ├───0011_submissionmodel_solve_count.py
    │   │   ├───0012_remove_submissionmodel_solve_count_and_more.py
    │   │   ├───0013_submissionmodel_time.py
    │   │   ├───0014_usermodel_batch_usermodel_department_usermodel_year.py
    │   │   ├───0015_usermodel_contest_attend_usermodel_problem_solve.py
    │   │   └───__init__.py
    │   ├───.DS_Store
    │   ├───__init__.py
    │   ├───admin.py
    │   ├───apps.py
    │   ├───authenticate.py
    │   ├───models.py
    │   ├───serializers.py
    │   ├───task.py
    │   ├───tests.py
    │   ├───urls.py
    │   ├───utils.py
    │   └───views.py
    ├───cpp/
    │   └───.DS_Store
    ├───.DS_Store
    ├───country.txt
    ├───get-pip.py
    ├───manage.py
    └───requirements.txt

### Contest Api

#### Create Contest
``` py
    def create_contest(request: Request):
    print(request.data)
    data = request.data
    contest = ContestModel(contest_name=data.get('contest_name'), duration=data.get('duration'),
                           start_at=data['start_at'],
                           end_at=data['end_at'], schedule_at=data['schedule_at'])
    contest.save()

    response = Response(
        create_success_response({"hello"}))
    return response
```

#### Upcoming Contest
``` py
    def upcoming_contest(request: Request):
    print(request.data)
    today = datetime.today()
    print(datetime.now())
    time = make_aware(datetime.now(), timezone=pytz.timezone("Asia/Dhaka"))
    contests = ContestModel.objects.filter(start_at__gte=time).all().values()

    for contest in contests:
        ans = False
        contest['is_active'] = ans
        contest['registered'] = ContestRegisterModel.objects.filter(contest_id=contest['id']).count()

    response = Response(
        create_success_response(contests))
    return response
```

#### All Contest
``` py
    contests = ContestModel.objects.filter(start_at__gte=time).all().values()
    response = Response(
        create_success_response(contests))
    return response
```

#### Previous Contest
``` py
    today = datetime.today()
    time = make_aware(datetime.now(), timezone=pytz.timezone("Asia/Dhaka"))
    contests = ContestModel.objects.filter(start_at__lte=time).all().values()

    for contest in contests:
        ans = False
        # print(contest['id'])
        contest['is_active'] = ans
        if UserModel.objects.filter(email=request.user).exists() and ContestRegisterModel.objects.filter(contest_id=contest['id'],
                                                                                                         user_id=UserModel.objects.get(
                                                                                                                 email=request.user).id).exists():
            ans = True
            contest['is_active'] = ans
        contest['registered'] = ContestRegisterModel.objects.filter(contest_id=contest['id']).count()

    response = Response(
        create_success_response(contests))
    return response
```

#### Contest Registration
``` py
    data = request.data
    if UserModel.objects.filter(email=request.user).exists():
        contest_registration = ContestRegisterModel(contest_id=ContestModel.objects.get(id=data['contest_id']),
                                                    user_id=UserModel.objects.get(email=request.user))
        contest_registration.save()
        return Response(create_success_response({}));
    return Response(create_error_response(200, {}))
```

#### Time Left
``` py
    time_left = ContestModel.objects.filter(id=request.data['contest_id']).first().end_at - timezone.now()
    time_left = time_left.total_seconds()
    return Response(create_success_response({"seconds": math.floor(time_left)}))
```

#### Process Analytics
``` py
    def process_analytics(request: Request):
        process_running = SubmissionModel.objects.filter(verdict_id=6).count()
        process_queue = SubmissionModel.objects.filter(verdict_id=2).count()
        process_finished = SubmissionModel.objects.count() - process_running - process_queue
        return Response(create_success_response({"running": process_running, "queue": process_queue, "finished": process_finished}))
```

### Problem API
#### Craete Problems 
``` py
    data = request.data
    problem = ProblemModel(problem_name=data['problem_name'], problem_statement=data['problem_statement'], input=data['input'],
                           output=data['output'], problem_number=data['problem_number'], time_limit=data['time_limit'], memory_limit=data['memory_limit'])
    problem.save()

    for testcase in data['testcases']:
        TestcaseModel(problem_id=problem, input=testcase['input'], output=testcase['output']).save()

    response = Response(
        create_success_response({"hello"}))
    return response
```

#### Get Problems 
``` py
    response = Response(
        create_success_response(ProblemModel.objects.all().values()))
    return response
```

#### Get Specific Problems 
``` py
    response = Response(
        create_success_response(ProblemModel.objects.filter(id=request.data['id']).all().values()))
    return response
```

#### Add Problem To contest 
``` py
    def add_problem_to_contest(request: Request):
        data = request.data
        ProblemConetestModel(problem_id=ProblemModel.objects.get(id=data['problem_id']), contest_id=ContestModel.objects.get(id=data['contest_id'])).save()
        response = Response(
            create_success_response("hello"))
        return response
```

#### Get Testcases 
``` py
    def get_test_cases(request: Request):
    data = request.data
    respose = TestcaseModel.objects.filter(problem_id=data['id']).all().values()
    return Response(create_success_response(respose))
```

#### Get Problem by Contest
``` py
    def contest_problem(request: Request):
    if str(request.user) != "AnonymousUser":
        print(request.data['id'])
        if ContestSubmissionModel.objects.filter(user__email=str(request.user), contest_id=request.data['id']).exists() is False:
            user = UserModel.objects.filter(email=str(request.user)).get()
            user.contest_attend = user.contest_attend + 1
            user.save()
        for problem in ProblemConetestModel.objects.filter(contest_id=request.data['id']):
            print(problem)
            if ContestSubmissionModel.objects.filter(contest_id=request.data['id'], user__email=str(request.user), problem_id=problem.problem_id_id).exists() is False:
                ContestSubmissionModel(contest_id=request.data['id'], user=UserModel.objects.get(email=request.user), problem_id=problem.problem_id_id).save()
        if PenaltyModel.objects.filter(contest_id=request.data['id'], user__email=str(request.user)).exists() is False:
            PenaltyModel(contest_id=request.data['id'], user=UserModel.objects.get(email=request.user)).save()
    data = request.data
    response = (ProblemConetestModel.objects.filter(contest_id=data['id']).order_by('problem_id__problem_number')
                .values('problem_id_id', 'problem_id__problem_number', 'problem_id__problem_name', 'problem_id__problem_statement', 'problem_id__input', 'problem_id__output', 'problem_id__memory_limit', 'problem_id__time_limit', 'problem_id__solve_count'))
    return Response(create_success_response(response))
```

#### Submission
``` py
    def submission(request: Request):
    data = request.data
    print(data)
    time_passed = timezone.now() - ContestModel.objects.filter(id=request.data['contest_id']).first().start_at
    time_passed = time_passed.total_seconds()
    time_passed = f'{int(time_passed / 3600):2}:{int((time_passed / 60) % 60):2}'
    submission = SubmissionModel(problem_id=request.data['problem_id'],
                                 contest_id=request.data['contest_id'], code=request.data['code'],
                                 verdict_id=2, language_id=1, verdict_text="In queue",
                                 time=time_passed,
                                 user_id=UserModel.objects.filter(email=request.user).get().id)
    submission.save()
    print(submission.id)
    test_func.delay(submission.id)
    return Response(create_success_response(SubmissionModel.objects.filter(id=submission.id).values()))
```

#### My Submission
``` py
    def mysubmission(request: Request):
    data = request.data
    print(request.user)
    response = SubmissionModel.objects.filter(contest_id=data['contest_id'], user_id=UserModel.objects.get(email=request.user).id).all().values('problem__problem_name', 'problem_id', 'verdict_text', 'problem__problem_number', 'time')
    return Response(create_success_response(response))
```

#### Submission
``` py
    def standing(request: Request):
    data = request.data
    ranking = PenaltyModel.objects.filter(contest_id=data['contest_id']).order_by('-solve', 'penalty').values('user_id', 'user__fullname', 'solve', 'penalty')
    for item in ranking:
        item['problem_status'] = ContestSubmissionModel.objects.filter(contest_id=data['contest_id'], user_id=item['user_id']).order_by('problem__problem_number').values()
    return Response(create_success_response(ranking))
```

### USER API

#### Create User
``` py
    def create_user(request: Request):
    data = request.data;
    email = data.get('email')
    user_info = email.split('@')
    batch = ""
    for i in range(len(user_info[0])):
        if '0' <= user_info[0][i] <= '9':
            batch = user_info[0][i:i+3]
            break
    trimester = "Spring"
    if batch[2] == '2':
        trimester = "Summer"
    if batch[2] == '3':
        trimester = "Fall"

    user = UserModel(fullname=data.get('fullname'), email=data.get('email'), username=str(random.random()),
                     gender=data.get('gender'), password=make_password(data.get
                                                                       ('password')), country=data.get('country'), batch=trimester, year=f'20{batch[0:2]}')
    user.save()
    refresh = RefreshToken.for_user(UserModel.objects.get(email=data.get('email')))
    response = Response(
        create_success_response({'access': str(refresh.access_token), 'refresh': str(refresh)}))
    response.set_cookie(
        key=settings.SIMPLE_JWT['AUTH_COOKIE'],
        value= str(refresh.access_token),
        expires=settings.SIMPLE_JWT['ACCESS_TOKEN_LIFETIME'],
        secure=settings.SIMPLE_JWT['AUTH_COOKIE_SECURE'],
        httponly=settings.SIMPLE_JWT['AUTH_COOKIE_HTTP_ONLY'],
        samesite=None
    )
    csrf.get_token(request)
    return response;
```

#### Sign In
``` py
    def signin(request: Request):
    user = UserModel.objects.get(email=request.data.get('email'))
    if check_password(request.data.get('password'), user.password) is False:
        return Response(create_error_response(200, {"hello": "gasasd"}))
    refresh = RefreshToken.for_user(UserModel.objects.get(email=request.data.get('email')))
    response = Response(
        create_success_response({'access': str(refresh.access_token), 'refresh': str(refresh)}))
    response.set_cookie(
        key=settings.SIMPLE_JWT['AUTH_COOKIE'],
        value= str(refresh.access_token),
        expires=settings.SIMPLE_JWT['ACCESS_TOKEN_LIFETIME'],
        secure=settings.SIMPLE_JWT['AUTH_COOKIE_SECURE'],
        httponly=settings.SIMPLE_JWT['AUTH_COOKIE_HTTP_ONLY'],
        samesite=None
    )
    csrf.get_token(request)
    return response
```

#### ME
``` py
    def me(request: Request):
    if request.user is None:
        return Response(create_error_response())
    return Response(create_success_response({"me": str(request.user)}))
```

#### Get Rank
``` py
    def get_rank(request: Request):
        q = Q()
        print(request.data)
        if request.data['gender']:
            q = q & Q(gender=request.data['gender'])
        if request.data['year']:
            q = q & Q(year=request.data['year'])
        if request.data['batch']:
            q = q & Q(batch=request.data['batch'])

        return Response(create_success_response(UserModel.objects.filter(q).order_by('-problem_solve', 'contest_attend').values('fullname', 'problem_solve', 'contest_attend')))
```




