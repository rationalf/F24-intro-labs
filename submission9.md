# Lab-9

## Task - 1

1) GitHub Actions allows us automate build tests and deployment pipeline.
2) I create file with name .github/workflows/github-actions-demo.yml and it creates new branch for this.
3) I check what create this file in Action tab.

### Part 2

1) I created changes in repository and push it.
2) But in actions doesn't change anything beacouse actions shows information in my way about master branch.

## Task - 2

1) I add 
on:
  workflow_dispatch:
2)I add 
- name: Gather System Information
        run: |
          echo "🖥️ System Information:"
          echo "===================="
          echo "Operating System: ${{ runner.os }}"
          echo "Runner Version: ${{ runner.name }} - ${{ runner.version }}"
          echo "Hardware Specifications:"
          echo "CPU: $(lscpu | grep 'Model name')"
          echo "Memory: $(free -h | grep 'Mem:')"
          echo "Disk Space: $(df -h | grep '/$')"
          echo "Kernel Version: $(uname -r)"
Output:
Run echo "🖥️ System Information:"
🖥️ System Information:
====================
Operating System: Linux
Runner Version: GitHub Actions 2 - 
Hardware Specifications:
CPU: Model name:                           AMD EPYC 7763 64-Core Processor
Memory: Mem:            15Gi       711Mi        13Gi        23Mi       1.1Gi        14Gi
Disk Space: /dev/root        73G   52G   21G  72% /
Kernel Version: 6.8.0-1014-azure
