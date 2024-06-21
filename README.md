This advanced task management and collaboration platform is designed to significantly enhance productivity and optimize workflow processes for both individuals and teams. Featuring an intuitive Kanban board interface, this platform is built to handle the complexity and nuances of modern project management needs.

Features
The following features have been implemented:

Kanban Board Interface: Manage tasks effortlessly with due dates, labels, and checklists.
My Tasks View: Consolidate all assigned tasks in a single, easy-to-navigate view.
Personal Projects: Create and manage projects independently.
Task Comments and Activity: Enhance team collaboration with integrated comments and activity tracking.
This project is still in active development, with many more features on the way. For updates on development, join our Discord server. Check out the Roadmap for planned features.

Installation
With Docker & Docker-Compose
Ensure you have Docker and Docker-Compose installed. Then follow these steps:

sh
Copy code
# Contributor Covenant Code of Conduct

## Our Pledge

In the interest of fostering an open and welcoming environment, we as
contributors and maintainers pledge to making participation in our project and
our community a harassment-free experience for everyone, regardless of age, body
size, disability, ethnicity, sex characteristics, gender identity and expression,
level of experience, education, socio-economic status, nationality, personal
appearance, race, religion, or sexual identity and orientation.

## Our Standards

Examples of behavior that contributes to creating a positive environment
include:

* Using welcoming and inclusive language
* Being respectful of differing viewpoints and experiences
* Gracefully accepting constructive criticism
* Focusing on what is best for the community
* Showing empathy towards other community members

Examples of unacceptable behavior by participants include:

* The use of sexualized language or imagery and unwelcome sexual attention or
 advances
* Trolling, insulting/derogatory comments, and personal or political attacks
* Public or private harassment
* Publishing others' private information, such as a physical or electronic
 address, without explicit permission
* Other conduct which could reasonably be considered inappropriate in a
 professional setting

## Our Responsibilities

Project maintainers are responsible for clarifying the standards of acceptable
behavior and are expected to take appropriate and fair corrective action in
response to any instances of unacceptable behavior.

Project maintainers have the right and responsibility to remove, edit, or
reject comments, commits, code, wiki edits, issues, and other contributions
that are not aligned to this Code of Conduct, or to ban temporarily or
permanently any contributor for other behaviors that they deem inappropriate,
threatening, offensive, or harmful.

## Scope

This Code of Conduct applies both within project spaces and in public spaces
when an individual is representing the project or its community. Examples of
representing a project or community include using an official project e-mail
address, posting via an official social media account, or acting as an appointed
representative at an online or offline event. Representation of a project may be
further defined and clarified by project maintainers.

## Enforcement

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported by contacting the project team at jordan@jordanthedev.com. All
complaints will be reviewed and investigated and will result in a response that
is deemed necessary and appropriate to the circumstances. The project team is
obligated to maintain confidentiality with regard to the reporter of an incident.
Further details of specific enforcement policies may be posted separately.

Project maintainers who do not follow or enforce the Code of Conduct in good
faith may face temporary or permanent repercussions as determined by other
members of the project's leadership.

## Attribution

This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4,
available at https://www.contributor-covenant.org/version/1/4/code-of-conduct.html

[homepage]: https://www.contributor-covenant.org

For answers to common questions about this code of conduct, see
https://www.contributor-covenant.org/faq
 && cd taskcafe
docker-compose -p taskcafe up -d
Visit http://localhost:3333 to complete the initial setup by creating the first system user.

From Source
Make sure Golang is installed on your machine. Then proceed with:

sh
Copy code
git clone https://github.com/JordanKnott/taskcafe && cd taskcafe
go run cmd/mage/main.go install
go run cmd/mage/main.go build
This process will:

Install Yarn packages for the frontend.
Build the React frontend and embed it in the binary.
Compile the final executable binary found in the dist folder.
Copy the example config file conf/app.example.toml to conf/app.toml and configure it accordingly. Run database migrations with:

sh
Copy code
taskcafe migrate
Launch the web interface with:

sh
Copy code
taskcafe web
For a detailed installation guide on Ubuntu/Debian, refer to the Wiki.

Comparison with Other Tools
Unlike other project management tools such as Trello or NextCloud, this platform is tailored to fit a unique workflow that prioritizes user preferences and enhances task management efficiency. While currently focused on delivering fundamental features, future updates will introduce advanced functionalities that distinguish this platform from its competitors.

Contributing & Community
Join our Discord server for support and community discussions. If you're interested in contributing, please read the Contribution Guide and adhere to our Code of Conduct.

License
This platform is licensed under the MIT License.
