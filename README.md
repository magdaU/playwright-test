# playwright-test
Playwright-test for dulux page

1.
Configuration add in dependiencies in Maven:
<dependencies>
  <dependency>
    <groupId>com.microsoft.playwright</groupId>
    <artifactId>playwright</artifactId>
    <version>1.44.0</version>
  </dependency>
  <dependency>
    <groupId>org.junit.jupiter</groupId>
    <artifactId>junit-jupiter</artifactId>
    <version>5.10.0</version>
    <scope>test</scope>
  </dependency>
</dependencies>

Add you need the Surefire Plugin to run tests with JUnit 5:
<build>
  <plugins>
    <plugin>
      <groupId>org.apache.maven.plugins</groupId>
      <artifactId>maven-surefire-plugin</artifactId>
      <version>3.0.0-M7</version>
    </plugin>
  </plugins>

 2. Install Playwright browsers

    Run this command in the terminal:  mvn exec:java -e -Dexec.mainClass=com.microsoft.playwright.CLI -Dexec.args="install"


3.  Recommended project structure

playwright-java/
├── pom.xml
└── src/
    └── test/
        └── java/
            └── ExampleTest.java


4. add a test
5. mvn test
6. Take a screenshot (optional)
   page.screenshot(new Page.ScreenshotOptions().setPath(Paths.get("screenshot.png")));


	📦 Optional: Add Page Object Model
If you plan to write many tests, it’s a good idea to use the Page Object Model


 
</build>
