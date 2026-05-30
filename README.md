# GymCoach

GymCoach is a private fitness app built with Flutter for iOS and Android, with a planned release for Google Play and the App Store. I built it to make strength training feel more structured from the first session to long-term progress, without splitting the experience across a plan generator, a workout logger, and a separate progress tracker.

The product is centered around a simple idea: a training app should help users decide what to do, guide them while they do it, and make the results easy to understand afterward. GymCoach is my attempt to make that flow feel consistent, personal, and practical.

## Hero Gallery

<p>
  <img src="screenshots/onboarding-plan-ready-1-en.png" alt="Plan ready screen" width="260" />
  <img src="screenshots/home-en.png" alt="Home screen" width="260" />
  <img src="screenshots/home-streak-en.png" alt="Home streak sheet" width="260" />
</p>
<p>
  <img src="screenshots/progress-overview-en.png" alt="Progress overview" width="260" />
  <img src="screenshots/progressive-overload-en.png" alt="Progressive overload" width="260" />
  <img src="screenshots/active-workout-en.png" alt="Active workout" width="260" />
</p>

Sample screenshots from the app are shown below using demo content. The UI supports both English and Hebrew, including RTL layouts.

## What GymCoach Does

- Personalizes the onboarding flow around training experience, schedule, equipment, muscle focus, and body context.
- Generates a starting training plan from that onboarding input and turns it into routines the user can actually follow.
- Gives users a home screen that keeps the current plan, training schedule, and quick actions in one place.
- Supports real workout logging with set-based and duration-based tracking inside an active workout flow.
- Closes each session with a completion summary and progression feedback that leads into longer-term adaptation.
- Tracks progress across workouts, exercise trends, weight trends, and strength-oriented milestones.
- Includes an exercise and program library so the app feels complete beyond the initial generated plan.
- Supports English and Hebrew across user-facing product areas.

## User Flow

Onboarding and plan generation happen once. After that, the main training loop repeats: home -> workout -> completion -> adaptation -> progress/history -> next session. Library, profile, and settings remain available throughout.

## Product Tour

### Onboarding And Personalization

The onboarding flow collects the training context needed to shape the first plan without turning first launch into a generic questionnaire.

<p>
  <img src="screenshots/onboarding-splash-en.png" alt="Onboarding splash" width="220" />
  <img src="screenshots/onboarding-gender-en.png" alt="Gender selection" width="220" />
  <img src="screenshots/onboarding-experience-en.png" alt="Experience selection" width="220" />
</p>
<p>
  <img src="screenshots/onboarding-days-en.png" alt="Training days selection" width="220" />
  <img src="screenshots/onboarding-equipment-en.png" alt="Equipment selection" width="220" />
  <img src="screenshots/onboarding-muscle-focus-en.png" alt="Muscle focus selection" width="220" />
</p>
<p>
  <img src="screenshots/onboarding-age-en.png" alt="Age step" width="220" />
  <img src="screenshots/onboarding-body-metrics-en.png" alt="Body metrics step" width="220" />
  <img src="screenshots/onboarding-comparison-en.png" alt="With GymCoach and without GymCoach comparison" width="220" />
</p>
<p>
  <img src="screenshots/onboarding-strength-chart-en.png" alt="Strength chart step" width="220" />
  <img src="screenshots/onboarding-trust-en.png" alt="Trust and privacy screen" width="220" />
</p>

Those screens set the boundaries for the plan generation step. I wanted the app to gather inputs that actually affect training structure, not just collect information for its own sake.

### Plan Generation

The generation step turns onboarding input into a concrete starting program the user can begin with immediately.

<p>
  <img src="screenshots/onboarding-generating-en.png" alt="Generating plan screen" width="220" />
  <img src="screenshots/onboarding-plan-ready-1-en.png" alt="Plan ready summary screen" width="220" />
  <img src="screenshots/onboarding-plan-ready-2-en.png" alt="Plan ready routine preview screen" width="220" />
  <img src="screenshots/onboarding-plan-ready-3-en.png" alt="Plan ready exercise breakdown screen" width="220" />
</p>

The goal here was to make the result feel usable and specific. A generated plan only matters if it becomes a clean workout structure that the user can understand and start following.

### Account And Sign-In

After the plan is ready, the app can hand the user into account creation or sign-in without making auth the center of the story.

<p>
  <img src="screenshots/auth-login-bottom-sheet-en.png" alt="Sign in options bottom sheet" width="220" />
  <img src="screenshots/auth-sign-up-en.png" alt="Sign up screen" width="220" />
</p>

This step is deliberately simple. It keeps the transition from first-run onboarding into the authenticated app clear without distracting from the training experience.

### Home And Workout Loop

This is the repeating day-to-day loop. The user should be able to open the app, see what is planned, start training, and stay oriented during the session.

<p>
  <img src="screenshots/home-en.png" alt="Home screen" width="220" />
  <img src="screenshots/home-streak-en.png" alt="Streak sheet" width="220" />
  <img src="screenshots/active-workout-en.png" alt="Active workout screen" width="220" />
</p>
<p>
  <img src="screenshots/home-mini-bar-en.png" alt="Home screen with minimized workout bar" width="220" />
  <img src="screenshots/workout-timer-en.png" alt="Workout timer sheet" width="220" />
  <img src="screenshots/workout-stopwatch-en.png" alt="Workout stopwatch sheet" width="220" />
</p>
<p>
  <img src="screenshots/completion-summary-en.png" alt="Workout completion summary" width="220" />
  <img src="screenshots/progressive-overload-en.png" alt="Progressive overload recommendation" width="220" />
</p>

I spent a lot of time on the active workout flow because that is where product intent meets operational detail. Logging sets, keeping the workout readable, making interruptions recoverable, and carrying the session into a clear completion moment all matter more than a flashy first-run moment.

### Progress And Adaptation

GymCoach tracks progress at more than one level. After the workout loop, the app needs to show overall trends, body-weight movement, and exercise-level history so users can understand what changed.

<p>
  <img src="screenshots/progress-overview-en.png" alt="Progress overview" width="220" />
  <img src="screenshots/weight-screen-en.png" alt="Weight trend screen" width="220" />
  <img src="screenshots/progress-exercises-en.png" alt="Exercise progress list" width="220" />
  <img src="screenshots/exercise-detail-en.png" alt="Exercise detail screen" width="220" />
</p>

The progress area is meant to be useful, not noisy. I wanted users to be able to read change over time, inspect specific exercises, and get practical progression guidance without digging through raw history.

### Library And Program Structure

The app is not only a workout logger. It also needs to support exercise browsing, program structure, and the day-to-day organization of routines in a way that still feels straightforward.

<p>
  <img src="screenshots/library-exercises-en.png" alt="Exercise library" width="220" />
  <img src="screenshots/library-exercises-filtered-en.png" alt="Filtered exercise library" width="220" />
  <img src="screenshots/program-detail-en.png" alt="Program detail screen" width="220" />
</p>
<p>
  <img src="screenshots/routine-detail-en.png" alt="Routine detail screen" width="220" />
  <img src="screenshots/edit-program-en.png" alt="Edit program screen" width="220" />
  <img src="screenshots/edit-routine-en.png" alt="Edit routine screen" width="220" />
</p>

Even outside the main workout flow, the app still needs to feel usable. The library views make it easier to inspect movements, filter by training focus, review how a program is organized, and see what each routine actually contains before starting it.

### Workout History And Settings

Smaller utility screens still matter because they shape whether the product feels dependable in regular use.

<p>
  <img src="screenshots/profile-workout-detail-en.png" alt="Workout detail history view" width="220" />
  <img src="screenshots/settings-en.png" alt="Settings screen" width="220" />
</p>

These screens are intentionally practical. They support history review, preferences, language, theme, units, and training-related defaults without trying to become their own separate product layer.

## Hebrew And RTL Support

GymCoach was built with English and Hebrew in mind. That affected layout, spacing, navigation, and screen composition early on, especially in dense views like active workouts and progress.

<p>
  <img src="screenshots/rtl-active-workout-he-dark.png" alt="Hebrew active workout" width="220" />
  <img src="screenshots/rtl-progress-he-dark.png" alt="Hebrew progress" width="220" />
  <img src="screenshots/rtl-settings-he.png" alt="Hebrew settings" width="220" />
</p>

## Tech Stack

- Flutter and Dart for the mobile app targeting iOS and Android
- Riverpod for app state and flow coordination
- Firebase Authentication for sign-in and user identity
- Cloud Firestore for user data, workouts, progress, and app state
- Firebase Functions for server-backed workflows
- `easy_localization` for English, Hebrew, and RTL support
- Shared and local persistence for settings, onboarding state, and workout recovery

## Product And Engineering Decisions

- I built GymCoach with Flutter because I wanted one shared mobile product surface targeting iOS and Android.
- The app follows a feature-oriented structure so product areas like onboarding, workout, progress, profile, and settings can evolve without collapsing into one giant UI layer.
- Riverpod is used for state management to keep screen logic, app state, and side effects more manageable as flows become interconnected.
- Firebase is used for authentication, data storage, and server-backed workflows where the app needs more than local state.
- Localization was treated as a product requirement, not a final pass, which is why English and Hebrew support appear across the core flows.
- The active workout flow was designed around persistence and recovery because workout sessions are easy to interrupt in real life.
- Analytics are wired through an internal abstraction so product visibility does not need to come at the cost of loose event handling.
- The AI-assisted plan generation flow is intentionally bounded. It exists to create a usable starting program inside a larger training product.

## Challenges I Had To Solve

One of the hardest parts was making onboarding detailed enough to generate something useful without making it feel heavy. It is easy for a fitness app to ask too many questions, and it is just as easy for the output to feel generic if the input is too shallow.

Another challenge was treating workouts as real sessions instead of static forms. The app has to handle timers, set logging, routine structure, progression logic, and interrupted app state in a way that still feels calm on screen. Progress was also tricky for a different reason: storing history is easy, but making the history readable and actionable is much harder.

RTL support also pushed a lot of decisions earlier in the build than I expected. Once dense screens are involved, localization affects layout, truncation, controls, and perceived polish very quickly.

## What I Learned

- Product decisions and engineering decisions shape each other more than they seem to at the start.
- A good fitness app needs consistency more than feature count. If the main training loop is not solid, everything around it feels weaker.
- AI features become much more useful when they are kept inside clear product boundaries.
- Localization is not just about strings. It changes spacing, composition, and flow design.
- Cross-platform mobile work gets better when state, interruption handling, and everyday usability are treated as first-class problems.

## Repository Note

This repository is a public overview only. GymCoach is an active private product, so the production source code remains private and proprietary while this repository documents the product and the engineering approach behind it.

Screenshots in this overview use sample or demo data. No source code, backend code, Firebase configuration, secrets, prompts, schemas, internal IDs, or private URLs are included here.
