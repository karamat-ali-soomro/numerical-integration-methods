# numerical-integration-methods
A simple interactive web application demonstrating the trapezoidal rule, Simpson's rule, and automatic step-size selection.

## Mathematical Methods

### 1. Trapezoidal Rule

The interval is divided into n subintervals of width

h = (b - a) / n.

The integral is approximated by

T_n = h [f(a)/2 + sum(f(a + ih), i = 1,...,n-1) + f(b)/2].

### 2. Simpson's Rule

Simpson's rule uses quadratic approximations and requires an even number of subintervals.

S_n = (h/3) [f(x_0) + 4 sum(f(x_i), odd i)
             + 2 sum(f(x_i), even interior i) + f(x_n)].

### 3. Automatic Step-Size Selection

The program refines the interval by doubling the number
of subintervals and estimates the error by comparing
successive approximations.

## Available Functions

- f(x) = x^2
- f(x) = sin(x)
- f(x) = e^x
- f(x) = x + 1

## How to Run

1. Download or clone this repository.
2. Open `index.html` in a web browser.
3. Select a function and enter the interval, n, and desired accuracy.
4. Click Calculate integral.

No additional packages are required.

## Technologies

- HTML
- CSS
- JavaScript

## Author

Karamat Ali

The formulas above are written in plain Markdown. You can improve their presentation later using LaTeX formatting in the README.

5. Publish a live demo

This is a particularly good step because your professor and future employers can try your application directly in their browsers.

Open your repository and click Settings.

In the sidebar, select Pages.

Under the build and deployment section, select Deploy from a branch.

Choose the main branch and the / (root) folder, then click Save.

Wait for GitHub Pages to publish your site. Your live link will generally look like https://YOUR-USERNAME.github.io/numerical-integration-methods/.

That URL is a template, not a verified live link. GitHub will show your actual published URL in the Pages settings. Keep index.html in the repository root.

6. Make your GitHub profile look professional

Your profile matters just as much as individual repositories. Since you are building a portfolio around mathematics, scientific computing and quantitative research, I recommend:

Bio: Mathematics | Scientific Computing | Numerical Methods | Quantitative Finance

Profile README: Create a public repository whose name exactly matches your GitHub username. Its README.md appears on your profile.

Pinned repositories: Pin your strongest projects rather than every assignment.

Project documentation: Explain the mathematics, implementation, testing, and limitations of each project.

Consistent quality: Use clear repository names, meaningful commit messages, and working code.

Over time, you can add stronger projects involving numerical analysis, inverse problems, physics-informed neural networks, and quantitative finance. Those will make your portfolio more distinctive than a profile containing only small classroom exercises.

7. What I recommend you do now

Complete these steps in order:

Create the public repository.
Upload index.html.
Add the README.
Test the application in your browser.
Publish it with GitHub Pages.
Add a screenshot and pin the repository to your profile.

One question: Do you already have a GitHub account with repositories on it, or will this be your very first repository? I can guide you through the next steps based on that.

I have a git bash can I use that ? in this way I will learn 

Yes! Using Git Bash is an excellent idea. You will learn how developers actually manage projects and upload them to GitHub. We can do everything from the terminal, step by step, and you will understand what each command does.

We will use your numerical integration assignment as your first project.

Step 1: Check Git is installed

Open Git Bash and enter:

git --version

You should see something like:

git version 2.x.x

Then check your Git identity:

git config --global user.name
git config --global user.email

These commands show the name and email Git uses to label your commits. If they are empty, we can configure them in the next step.

Step 2: Create your project folder

Let's keep your project organized in a folder named numerical-integration-methods.

Enter these commands one at a time:

cd ~/Desktop
mkdir numerical-integration-methods
cd numerical-integration-methods

What each command does:

Command

	

Meaning




cd

	

Move into a folder




mkdir

	

Create a new folder




pwd

	

Show your current folder




ls

	

List files and folders

Now enter:

pwd

Your path should end with something like:

/Desktop/numerical-integration-methods

If your Desktop is not inside your Git Bash home directory, don't worry; we can adjust the path.

Step 3: Put your HTML file in this folder

Download the HTML file I created earlier:

Download numerical_integration.html

Move it into your numerical-integration-methods folder and rename it to index.html.

Then, in Git Bash, run:

ls

You should see:

index.html
Step 4: Initialize Git

Run:

git init

This creates a local Git repository in your project folder.

Now run:

git status

Git should show index.html as an untracked file.

What does that mean? Git can see the file, but it is not tracking it in the repository's history yet.

Step 5: Make your first commit

Run:

git add index.html
git commit -m "Add numerical integration application"

Here is what these commands mean:

git add — selects the file to include in the next commit.

git commit — saves a snapshot of the selected changes.

-m — lets you write a short description of the commit.

Check the result:

git log --oneline

You should see your first commit.

Step 6: Connect it to GitHub

We will do this after the local project is ready.

First, create a new empty public repository on 
GitHub
 named:

numerical-integration-methods

Do not initialize it with a README, license, or .gitignore; we will create those locally and upload them from Git Bash.

Then we will connect your local repository to GitHub using commands like:

git remote add origin https://github.com/YOUR-USERNAME/numerical-integration-methods.git
git branch -M main
git push -u origin main

Replace YOUR-USERNAME with your actual GitHub username. GitHub may ask you to authenticate.

Your task right now

Let's learn this properly instead of running everything at once.

Do Steps 1–4 first. Then send me the output of these two commands:

pwd
ls

I will check that your folder and file are correct before we move to commits and GitHub.
