# How to set up Ubuntu for Hugging Face chatbot development in python

1. Install Python 3:

   ```
   sudo apt update
   sudo apt install python3 python3-pip python3-venv
   ```

2. Create a virtual environment:

   ```
   python3 -m venv chatbot_env
   source chatbot_env/bin/activate
   ```

3. Install required libraries:

   ```
   pip install transformers torch datasets accelerate
   ```

4. Install additional dependencies:

   ```
   sudo apt install python3-dev build-essential
   ```

5. Install Jupyter Notebook (optional but useful):

   ```
   pip install jupyter
   ```

6. Install Git:

   ```
   sudo apt install git
   ```

7. Clone the Hugging Face transformers repository:

   ```
   git clone https://github.com/huggingface/transformers.git
   ```

8. Install additional Hugging Face libraries:

   ```
   pip install tokenizers sentencepiece sacremoses
   ```

9. Set up CUDA if you have an NVIDIA GPU (optional):
   - Install NVIDIA drivers
   - Install CUDA toolkit
   - Install cuDNN

10. Configure your development environment:
    - Set up a code editor like VSCode or PyCharm
    - Configure linters and formatters (e.g., flake8, black)

11. Test your setup:

    ```python
    from transformers import pipeline
    classifier = pipeline("sentiment-analysis")
    result = classifier("Hello, world!")
    print(result)
    ```

Remember to activate your virtual environment (`source chatbot_env/bin/activate`) whenever you're working on your chatbot project. This setup provides a solid foundation for developing Hugging Face chatbots on Ubuntu.

<!-- Citations:
[1] <https://www.geeksforgeeks.org/how-to-install-python-in-ubuntu/>
[2] <https://phoenixnap.com/kb/how-to-install-python-3-ubuntu>
[3] <https://www.eukhost.com/kb/how-to-install-and-switch-python-versions-on-ubuntu-22-04/>
[4] <https://docs.python-guide.org/starting/install3/linux/>
[5] <https://www.youtube.com/watch?v=9QftEX6yZP4>
[6] <https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server>
[7] <https://discuss.python.org/t/install-python-3-11-9-on-ubuntu/51093>
[8] <https://forums.docker.com/t/how-to-run-multiple-wordpress-instances-using-docker/94836> -->
