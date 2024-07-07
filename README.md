Project Workflow Documentation:

Overview:
This README outlines the workflow I implemented for managing multiple repositories using GitHub, aimed at streamlining the development process and enhancing collaboration. The setup involves using submodules, automated workflows, and secure environment management.

Research:
Before beginning the implementation, I conducted thorough research to ensure a robust setup. I referred to GitHub's official documentation, various instructional videos on YouTube, and numerous discussions on Stack Overflow. Additionally, I consulted directly with the client, Charbel, to fully understand and align with the project requirements.

Implementation:

    Initial Setup:
        Repositories Initialization: Created two main repositories, RepoA and RepoB, and initialized them with a main branch each.
        GitManage Repository: Established a third repository named GitManage, which incorporates RepoA and RepoB as submodules, allowing centralized control and updates.
        Configuration and Workflow Integration
        Configuration Management:

Created a config.yaml file in each repository to manage configuration variables.

Python Integration:

    Developed a Python script in both RepoA and RepoB to dynamically read from the config.yaml file

Security with PATs:

    Generated a Personal Access Token (PAT) with necessary permissions and safely stored it in GitHub secrets to manage access and operations securely across repositories.

Automated Workflows:

    Individual Repo Workflows: Set up workflows in RepoA and RepoB that trigger on push events, sending notifications to GitManage for updates.
    GitManage Workflow: Implemented a workflow in GitManage that reacts to these notifications by updating and merging changes in the submodules.

Challenges:

    Documentation Navigation: Initially, skimming through the extensive GitHub documentation took considerable time.
    Repository Permissions: Faced challenges in writing to the repository through GitHub Actions. Resolved this issue by refining the workflow permissions and utilizing solutions found on Stack Overflow.

Conclusion:

    This workflow efficiently manages multiple repositories, ensuring streamlined development and easy updates.
