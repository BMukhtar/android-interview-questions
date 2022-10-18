<p align="center">
<img alt="AndroidInterviewQuestions" src="https://raw.githubusercontent.com/MindorksOpenSource/android-interview-questions/master/assets/banner-android-interview-questions.jpg">
</p>

# Android Interview Questions
[![MindOrks](https://img.shields.io/badge/mindorks-opensource-blue.svg)](https://mindorks.com/open-source-projects)
[![MindOrks Community](https://img.shields.io/badge/join-community-blue.svg)](https://mindorks.com/join-community)
[![MindOrks Android Store](https://img.shields.io/badge/Mindorks%20Android%20Store-Android%20Interview%20Questions-blue.svg?style=flat)](https://mindorks.com/android/store)

> Android Interview Questions - Your Cheat Sheet For Android Interview

## Prepared and maintained by [Amit Shekhar](https://github.com/amitshekhariitbhu) who is having experience of taking interviews of many Android developers and cracking interviews of top companies.

<p align="center">
<a href="https://mindorks.com/android-app-development-online-course" target="_blank">
  <img alt="Android Roadmap" src="https://raw.githubusercontent.com/MindorksOpenSource/android-interview-questions/master/assets/roadmap.png">
</a>	
</p>

## A complete guide for learning Android Development - [Check here](https://mindorks.com/android-app-development-online-course)

## Contents

* [Core Android](#core-android)
* [Android Libraries](#android-libraries)
* [Android Architecture](#android-architecture)
* [Android Design Problem](#android-design-problem)
* [Android Unit Testing](#android-unit-testing)
* [Android Tools And Technologies](#android-tools-and-technologies)
* [Java and Kotlin](#java-and-kotlin)
* [Data Structures And Algorithms](#data-structures-and-algorithms)
* [Other Topics](#other-topics)

### Core Android

#### Base

* **Tell all the Android application components.** - [Learn from here](https://developer.android.com/guide/components/fundamentals.html#Components)

* **What is the project structure of an Android Application?** - [Learn from here](https://developer.android.com/studio/projects)

* **What is `Context`? How is it used?** - [Learn from here](https://blog.mindorks.com/understanding-context-in-android-application-330913e32514)

* **What is `AndroidManifest.xml`?** - [Learn from here](https://developer.android.com/guide/topics/manifest/manifest-intro)

* **What is `Application` class?**
    - The Application class in Android is the base class within an Android app that contains all other components such as activities and services. The Application class, or any subclass of the Application class, is instantiated before any other class when the process for your application/package is created.

#### Activity and Fragment

* **What is `Activity` and its lifecycle?** - [Learn from here](https://www.youtube.com/watch?v=RiFui-i-s-o)

* **What is the difference between onCreate() and onStart()** - [Learn from here](https://www.youtube.com/watch?v=RiFui-i-s-o)

* **When only onDestroy is called for an activity without onPause() and onStop()?** - [Learn from here](https://www.youtube.com/watch?v=QSxcLnZ1-RU)

* **Why do we need to call setContentView() in onCreate() of Activity class?** - [Learn from here](https://www.youtube.com/watch?v=zeYK8JdMOi8)

* **What is onSavedInstanceState() and onRestoreInstanceState() in activity?**
    - onSavedInstanceState() - This method is used to store data before pausing the activity.
    - onRestoreInstanceState() - This method is used to recover the saved state of an activity when the activity is recreated after destruction. So, the onRestoreInstanceState() receive the bundle that contains the instance state information.

* **What is `Fragment` and its lifecycle.** - [Learn from here](https://blog.mindorks.com/android-fragments-and-its-lifecycle)

* **What are "launch modes"?** - [Learn from here](https://blog.mindorks.com/android-activity-launchmode-explained-cbc6cf996802)

* **What is the difference between a `Fragment` and an `Activity`? Explain the relationship between the two.** - [Learn from here](https://stackoverflow.com/questions/10478233/why-fragments-and-when-to-use-fragments-instead-of-activities)

* **When should you use a Fragment rather than an Activity?**
    - When you have some UI components to be used across various activities
    - When multiple view can be displayed side by side just like viewPager

* **What is the difference between adding/replacing fragment in backstack?** - [Learn from here](https://stackoverflow.com/questions/24466302/basic-difference-between-add-and-replace-method-of-fragment/24466345)

* **Why is it recommended to use only the default constructor to create a `Fragment`?** - [Learn from here](https://www.youtube.com/watch?v=9EdvcycKP9A)

* **How would you communicate between two Fragments?** - [Learn from here](https://blog.mindorks.com/how-to-communicate-between-fragments)

* **What is retained `Fragment`?**
    - By default, Fragments are destroyed and recreated along with their parent Activity’s when a configuration change occurs. Calling setRetainInstance(true) allows us to bypass this destroy-and-recreate cycle, signaling the system to retain the current instance of the fragment when the activity is recreated.

* **What is the purpose of `addToBackStack()` while commiting fragment transaction?**
    - By calling addToBackStack(), the replace transaction is saved to the back stack so the user can reverse the transaction and bring back the previous fragment by pressing the Back button. For more [Learn from here](https://stackoverflow.com/questions/22984950/what-is-the-meaning-of-addtobackstack-with-null-parameter)

#### Views and ViewGroups

* **What is `View` in Android?** - [Learn from here](https://blog.mindorks.com/android-user-interface-view-components)

* **Difference between `View.GONE` and `View.INVISIBLE`?** - [Learn from here](https://stackoverflow.com/questions/11556607/android-difference-between-invisible-and-gone)

* **Can you a create custom view? How?** - [Learn from here](https://blog.mindorks.com/create-your-own-custom-view)

* **What are ViewGroups and how they are different from the Views?**
    - View: View objects are the basic building blocks of User Interface(UI) elements in Android. View is a simple rectangle box which responds to the user’s actions. Examples are EditText, Button, CheckBox etc. View refers to the android.view.View class, which is the base class of all UI classes.
    - ViewGroup: ViewGroup is the invisible container. It holds View and ViewGroup. For example, LinearLayout is the ViewGroup that contains Button(View), and other Layouts also. ViewGroup is the base class for Layouts.

* **What is a Canvas?** - [Learn from here](https://blog.mindorks.com/understanding-canvas-api-in-android)

* **Tell about Constraint Layout** - [Learn from here](https://blog.mindorks.com/using-constraint-layout-in-android-531e68019cd)

* **Do you know what is the view tree? How can you optimize its depth?** - [Learn from here](https://developer.android.com/reference/android/view/ViewTreeObserver)

* **How does the Touch Control and Events work in Android?** - [Learn from here](https://blog.mindorks.com/touch-control-and-events-in-android) and [here](https://www.youtube.com/watch?v=tKeYr7iV5xE)

#### Displaying Lists of Content

* **How does RecyclerView work internally?** - [Learn from here](https://blog.mindorks.com/how-does-recyclerview-work-internally) and [here](https://www.youtube.com/watch?v=60IYWdnHsZI)

* **What is the ViewHolder pattern? Why should we use it?** - [Learn from here](https://stackoverflow.com/questions/21501316/what-is-the-benefit-of-viewholder-pattern-in-android)

* **RecyclerView Optimization - Scrolling Performance Improvement** - [Learn from here](https://blog.mindorks.com/recyclerview-optimization)

* **What is `SnapHelper`?** - [Learn from here](https://blog.mindorks.com/using-snaphelper-in-recyclerview-fc616b6833e8)

#### Dialogs and Toasts

* **What is `Dialog` in Android?** - [Learn from here](https://developer.android.com/guide/topics/ui/dialogs)

* **What is `Toast` in Android?** - [Learn from here](https://developer.android.com/guide/topics/ui/notifiers/toasts)

* **What the difference between `Dialog` and `Dialog Fragment`?** - [Learn from here](https://stackoverflow.com/questions/7977392/android-dialogfragment-vs-dialog)

#### Intents and Broadcasting

* **What is `Intent`?** - [Learn from here](https://blog.mindorks.com/what-are-intents-in-android)

* **What is an Implicit `Intent`?** - [Learn from here](https://blog.mindorks.com/what-are-intents-in-android)
        
* **What is an Explicit `Intent`?** - [Learn from here](https://blog.mindorks.com/what-are-intents-in-android)

* **What is the function of an `IntentFilter`?** - [Learn from here](https://developer.android.com/reference/android/content/IntentFilter)

* **What is a `PendingIntent`?**
    - If you want someone to perform any Intent operation at future point of time on behalf of you, then we will use Pending Intent.

#### Inter-process Communication

* **How can two distinct Android apps interact?** - [Learn from here](https://developer.android.com/training/basics/intents)

* **Is it possible to run an Android app in multiple processes? How?** - [Learn from here](https://stackoverflow.com/questions/6567768/how-can-an-android-application-have-more-than-one-process)

* **What can you use for background processing in Android?** - [Learn from here](https://developer.android.com/guide/background)

* **What is a `ContentProvider` and what is it typically used for?** - [Learn from here](https://developer.android.com/guide/topics/providers/content-provider-basics) and [here](https://developer.android.com/guide/topics/providers/content-providers)

#### Long-running Operations

* **How to run parallel tasks in Java or Android, and get callback when all complete?** - [Learn from here](https://www.youtube.com/watch?v=v0ZSnISeyKE)

* **Why should you avoid to run non-ui code on the main thread?** - [Learn from here](https://developer.android.com/training/multiple-threads/communicate-ui)

* **What is ANR? How can the ANR be prevented?** - [Learn from here](https://developer.android.com/topic/performance/vitals/anr.html)

* **What is a `Loader`? (Deprecated)** - [Learn from here](https://developer.android.com/guide/components/loaders)

* **What is the relationship between the life cycle of an `AsyncTask` and an `Activity`? What problems can this result in? How can these problems be avoided?**
    - An AsyncTask is not tied to the life cycle of the Activity that contains it. So, for example, if you start an AsyncTask inside an Activity and the user rotates the device, the Activity will be destroyed (and a new Activity instance will be created) but the AsyncTask will not die but instead goes on living until it completes.
    
    - Then, when the AsyncTask does complete, rather than updating the UI of the new Activity, it updates the former instance of the Activity (i.e., the one in which it was created but that is not displayed anymore!). This can lead to an Exception (of the type java.lang.IllegalArgumentException: View not attached to window manager if you use, for instance, findViewById to retrieve a view inside the Activity).
    
    - There’s also the potential for this to result in a memory leak since the AsyncTask maintains a reference to the Activity, which prevents the Activity from being garbage collected as long as the AsyncTask remains alive.

    - For these reasons, using AsyncTasks for long-running background tasks is generally a bad idea . Rather, for long-running background tasks, a different mechanism (such as a service) should be employed.
    
    - Note: AsyncTasks by default run on a single thread using a serial executor, meaning it has only 1 thread and each task runs one after the other.

* **Explain `Looper`, `Handler` and `HandlerThread`.** - [Learn from here](https://blog.mindorks.com/android-core-looper-handler-and-handlerthread-bd54d69fe91a) and [from video](https://www.youtube.com/watch?v=rfLMwbOKLRk&list=PL6nth5sRD25hVezlyqlBO9dafKMc5fAU2)

* **How does the threading work in Android?** - [Learn from here](https://www.youtube.com/watch?v=zfDYK-xB1Uo)

* **Android Memory Leak and Garbage Collection** - [Learn from here](https://www.youtube.com/watch?v=zCSSFRRIreo)

#### Data Saving

* **How to persist data in an Android app?** - [Learn from here](https://blog.mindorks.com/android-shared-preferences-in-kotlin)

* **How would you preserve `Activity` state during a screen rotation?** - [Learn from here](https://stackoverflow.com/questions/3915952/how-to-save-state-during-orientation-change-in-android-if-the-state-is-made-of-m)

* **What are different ways to store data in your Android app?** - [Learn from here](https://blog.mindorks.com/understanding-storage-system-to-store-data-in-android)

* **Explain Scoped Storage in Android.** - [Learn from here](https://blog.mindorks.com/understanding-the-scoped-storage-in-android)

* **How to encrypt data in Android?** - [Learn from here](https://blog.mindorks.com/how-to-encrypt-data-safely-on-device-and-use-the-androidkeystore)

* **What is commit() and apply() in SharedPreferences?**
    - commit() returns a boolean value of success or failure immediately by writing data synchronously.
    - apply() is asynchronous and it won't return any boolean response. If you have an apply() outstanding and you are performing commit(), then the commit() will be blocked until the apply() is not completed.

#### Look and Feel

* **How to generate dynamic colors based in image?** - [Learn from here](https://blog.mindorks.com/color-palette-in-android)

* **Explain about Density Independence Pixel** - [Learn from here](https://blog.mindorks.com/understanding-density-independent-pixel-sp-dp-dip-in-android)

* **How do you find memory leaks in Android applications?** - [Learn from here](https://blog.mindorks.com/practical-guide-to-solve-out-of-memory-error-in-android-application) and [here](https://mindorks.com/blog/detecting-and-fixing-memory-leaks-in-android)

#### Supporting Different Screen Sizes

* **How do you support different types of resolutions?** - [Learn from here](https://developer.android.com/training/multiscreen/screensizes)

#### Android Jetpack

* **What is Android Jetpack and why to use this?** - [Learn from here](https://blog.mindorks.com/what-is-android-jetpack-and-why-should-we-use-it)

* **What are Android Architecture Components?** - [Learn from here](https://blog.mindorks.com/what-are-android-architecture-components)

* **What is LiveData in Android?** - [Learn from here](https://blog.mindorks.com/understanding-livedata-in-android)

* **How LiveData is different from ObservableField?** - [Learn from here](https://blog.mindorks.com/livedata-vs-observable-in-android)

* **What is the difference between setValue and postValue in LiveData?** - [Learn from here](https://blog.mindorks.com/livedata-setvalue-vs-postvalue-in-android)

* **How to share ViewModel between Fragments in Android?** - [Learn from here](https://blog.mindorks.com/shared-viewmodel-in-android-shared-between-fragments)

* **Explain Work Manager in Android.** - [Learn from here](https://blog.mindorks.com/integrating-work-manager-in-android)

* **Use-cases of WorkManager in Android.** - [Learn from here](https://www.youtube.com/watch?v=4LTpYXFMnJw)

* **How ViewModel work internally?** - [Learn from here](https://blog.mindorks.com/android-viewmodels-under-the-hood)

#### Others

* **How do you troubleshoot a crashing application?** - [Learn from here](https://developer.android.com/topic/performance/vitals/crash)

* **What is Android Data Binding?** - [Learn from here](https://developer.android.com/topic/libraries/data-binding/index.html)

### Android Libraries

* **Why do we use the Dependency Injection Framework like Dagger in Android?** - [Learn from here](https://blog.mindorks.com/why-do-we-use-the-dependency-injection-framework-in-android)

* **How does the Dagger work?** - [Learn from here](https://blog.mindorks.com/android-annotation-processing-tutorial-part-1-a-practical-approach) and [here]((https://www.youtube.com/watch?v=Grzqz-B3NWU))

* **What is Component in Dagger?** - [Learn from here](https://www.youtube.com/watch?v=Grzqz-B3NWU)

* **What is Module in Dagger?** - [Learn from here](https://www.youtube.com/watch?v=Grzqz-B3NWU)

* **What is Flow in Kotlin?** - [Learn from here](https://blog.mindorks.com/what-is-flow-in-kotlin-and-how-to-use-it-in-android-project)

### Android Architecture

* **Describe MVVM.** - [Learn from here](https://blog.mindorks.com/mvvm-architecture-android-tutorial-for-beginners-step-by-step-guide) and [here](https://www.youtube.com/watch?v=HJMZNF-tG-4)

* **What is presenter?** - [Learn from here](https://mindorks.com/course/android-mvp-introduction)

* **What is model?** - [Learn from here](https://mindorks.com/course/android-mvp-introduction)

* **Describe the repository pattern** - [Learn from here](https://blog.mindorks.com/android-mvp-architecture-extension-with-interactors-and-repositories-bd4b51972339)

* **Tell something about clean code** - [Learn from here](https://blog.mindorks.com/every-programmer-should-read-this-book-6755dedec78d)


### Android Unit Testing

* **Explain unit test.** - [Learn from here](https://developer.android.com/training/testing/unit-testing/local-unit-tests)

* **Have you done unit testing or automatic testing?**

* **Why mockk (new alternative of Mockito) is used** [Learn from here](https://mockk.io/)

* **Describe JUnit test.** - [Learn from here](https://en.wikipedia.org/wiki/JUnit)

* **Describe code coverage.** - [Learn from here](https://blog.mindorks.com/generate-global-code-coverage-report-in-android-development-using-jacoco-plugin)

### Android Tools And Technologies

* **What is ADB?** - [Learn from here](https://developer.android.com/studio/command-line/adb)

* **What is Lint? What is it used for?** - [Learn from here](https://blog.mindorks.com/what-is-lint-what-is-it-used-for)

* **Git.** - [Learn from here](https://www.youtube.com/watch?v=D4h8Dbrjt4M&list=PL6nth5sRD25itbyNVUULAebzL-VLrLfkK)

* **Android Development Useful Tools.** - [Learn from here](https://blog.mindorks.com/android-development-useful-tools-fd73283e82e3)

* **Firebase.** - [Learn from here](https://firebase.google.com/)

* **How to use Firebase realtime database in your app?** - [Learn from here](https://blog.mindorks.com/firebase-realtime-database-android-tutorial)

* **What is Gradle?** - [Learn from here](https://blog.mindorks.com/gradle-for-android-developers-getting-the-most-of-it)

### Kotlin

#### OOP

* **Explain OOP Concepts.**
    - Object-Oriented Programming is a methodology of designing a program using classes, objects, 
    [inheritance](https://en.wikipedia.org/wiki/Inheritance_(object-oriented_programming)),
    [polymorphism](https://en.wikipedia.org/wiki/Polymorphism_(computer_science)),
    [abstraction](https://en.wikipedia.org/wiki/Abstraction_(software_engineering)), and
    [encapsulation](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)).

* **Tell some advantages of Kotlin.** - [Learn from here](https://www.youtube.com/watch?v=kRhivT-jKzY&t=16s)

* **What is the difference between `val` and `var`?** - [Learn from here](https://stackoverflow.com/questions/44200075/val-and-var-in-kotlin)

* **What is the difference between `const` and `val`?** - [Learn from here](https://blog.mindorks.com/what-is-the-difference-between-const-and-val)

* **How to ensure `null` safety in Kotlin?** - [Learn from here](https://blog.mindorks.com/safecalls-vs-nullchecks-in-kotlin)

* **When to use `lateint` keyword used in Kotlin?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-lateinit-vs-lazy)

* **How to check if a `lateinit` variable has been initialized?** - [Learn from here](https://blog.mindorks.com/how-to-check-if-a-lateinit-variable-has-been-initialized)

* **How to do lazy initialization of variables in Kotlin?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-lateinit-vs-lazy) and [here](https://www.youtube.com/watch?v=yEX9_PeNRy4)

* **What are `companion objects` in Kotlin?** - [Learn from here](https://blog.mindorks.com/companion-object-in-kotlin)

* **What are the visibility modifiers in Kotlin?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-visibility-modifiers-private-protected-internal-public)

* **What is the equivalent of Java static methods in Kotlin?** - [Learn from here](https://blog.mindorks.com/what-is-the-equivalent-of-java-static-methods-in-kotlin)

* **What is a data class in Kotlin?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-data-class)

* **How to create a Singleton class in Kotlin?** - [Learn from here](https://blog.mindorks.com/how-to-create-a-singleton-class-in-kotlin)

* **What is the difference between `open` and `public` in Kotlin?** - [Learn from here](https://blog.mindorks.com/understanding-open-keyword-in-kotlin)

* **Explain the use-case of `let`, `run`, `with`, `also`, `apply` in Kotlin.** - [Learn from here](https://blog.mindorks.com/using-scoped-functions-in-kotlin-let-run-with-also-apply) and [here](https://www.youtube.com/watch?v=AiFBEH54Xpw)

* **Difference between List and Array types in Kotlin** - [Learn from here](https://blog.mindorks.com/difference-between-list-and-array-types-in-kotlin)

* **What are `Labels` in Kotlin?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-returns-jumps-labels)

* **What is an `Init` block in Kotlin?** - [Learn from here](https://blog.mindorks.com/understanding-init-block-in-kotlin)

* **Explain `pair` and `triple` in Kotlin.** - [Learn from here](https://blog.mindorks.com/pair-and-triple-in-kotlin)

* **How to choose between `apply` and `with`?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-apply-vs-with)

* **How to choose between `switch` with `when`?** - [Learn from here](https://blog.mindorks.com/replace-switch-with-when-in-kotlin)

* **What are Coroutines in Kotlin?** - [Learn from here](https://blog.mindorks.com/mastering-kotlin-coroutines-in-android-step-by-step-guide)

* **What is Coroutine Scope?** - [Learn from here](https://blog.mindorks.com/mastering-kotlin-coroutines-in-android-step-by-step-guide)

* **What is Coroutine Context?** - [Learn from here](https://blog.mindorks.com/mastering-kotlin-coroutines-in-android-step-by-step-guide)

* **Launch vs Async in Kotlin Coroutines** - [Learn from here](https://www.youtube.com/watch?v=nC30UiDv8Xc)

* **What is inline function in Kotlin?** - [Learn from here](https://blog.mindorks.com/understanding-inline-noinline-and-crossinline-in-kotlin)

* **When to use Kotlin sealed classes?** - [Learn from here](https://blog.mindorks.com/learn-kotlin-sealed-classes)

* **Explain function literals with receiver in Kotlin?** - [Learn from here](https://blog.mindorks.com/function-literals-with-receiver-in-kotlin)

* **What are higher-order functions in Kotlin?** - [Learn from here](https://blog.mindorks.com/understanding-higher-order-functions-and-lambdas-in-kotlin)

* **What are Lambdas in Kotlin** - [Learn from here](https://blog.mindorks.com/understanding-higher-order-functions-and-lambdas-in-kotlin)

### License
```
   Copyright (C) 2020 MINDORKS NEXTGEN PRIVATE LIMITED

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

### Contributing to Android Interview Questions
Just make pull request. You are in!
