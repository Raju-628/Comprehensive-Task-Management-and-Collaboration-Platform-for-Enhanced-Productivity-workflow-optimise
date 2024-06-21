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
git clone https://github.com/JordanKnott/taskcafe && cd taskcafe
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
