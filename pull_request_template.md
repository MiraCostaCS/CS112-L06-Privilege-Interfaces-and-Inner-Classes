## 📋 Project Assessment: Lab #6 - Privilege + Interfaces and Inner Classes

### 1. Git & Workflow
- [ ] **Commit Messages:** Descriptive and incremental (e.g., "Implemented Comparable interface in Person class").
- [ ] **Refactoring:** Completed all `TODO:` markers and updated dependent code across `Person.java` and `Main.java`.

### 2. Functional Requirements

#### Part 1: Implementing `Comparable`
- [ ] **`Person.java` Implementation:**
    - [ ] Added `implements Comparable<Person>` (or `Comparable`) to class header.
    - [ ] Does not create `Comparable.java` interface but uses built in `java.lang.Comparable`
    - [ ] Implemented `@Override compareTo()` method using privilege points for natural ordering.
- [ ] **`Main.java` (Option 3 - Compare with Others):**
    - [ ] Option 3 loops through preloaded array of users.
    - [ ] Explicitly uses `compareTo()` method to evaluate and display relative privilege ("More privilege than...", "Less privilege than...").

#### Part 2: Upgrading to `Identity` Inner Class
- [ ] **`Identity` Inner Class (`Person.java`):**
    - [ ] Defined inner class `Identity` with `pronouns` (`String`) and `background` (`String`).
    - [ ] Created 2 constructors for `Identity`: default and full parameters (`pronouns`, `background`).
    - [ ] Overrode `toString()` and `equals()` inside `Identity`.
- [ ] **Refactoring `Person` Outer Class:**
    - [ ] Updated `story` instance variable type from `String` to `Identity`.
    - [ ] Refactored constructors (Default, Full, Copy) to instantiate/deep copy `Identity`.
    - [ ] Updated/added getters and setters: `setPronouns()`, `setBackground()`, `getPronouns()`, `getBackground()`.
    - [ ] Refactored `toString()` and `equals()` to delegate identity field checks to the `Identity` class.
- [ ] **Refactoring `Main.java` Driver:**
    - [ ] Updated `fillInfo()` method to collect pronouns and background identity statement.
    - [ ] Displayed preferred pronoun examples during user input prompt.
    - [ ] Properly invoked updated setters/constructors on the `Person` object.

### 3. Code Quality & OOP Standards
- [ ] **Encapsulation:** Instance variables in both `Person` and `Identity` remain `private`.
- [ ] **Deep Copying:** Enforced in copy constructors and setters for the `Identity` object.
- [ ] **Annotations:** `@Override` tag placed above `compareTo()`, `toString()`, and `equals()`.
- [ ] **Naming & Style:** `camelCase` for methods/variables; `PascalCase` for classes; consistent indentation.

### 4. Hacker Challenge (Optional)
- [ ] **Visual ASCII Representation:** Implemented ASCII scale visualization showing relative positioning of privilege estimates.
- [ ] **Extended Questionnaire:** Expanded question set to cover more axes of privilege (Yes/No format).
- [ ] **Expanded `Identity` Model:** Added opt-in identity metrics (e.g., race, nationality, sexuality) with user opt-out support.
