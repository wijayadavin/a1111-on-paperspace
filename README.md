# [Automatic 1111 WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) on [Paperspace](https://www.paperspace.com)

## Usage (Using Notebook)
1. On [Paperspace terminal](https://docs.paperspace.com/gradient/notebooks/terminal/) run:
    ```
    git clone https://github.com/wijayadavin/a1111-on-paperspace.git
    ```

2. Run [launch.ipynb](launch.ipynb) to launch Automatic 1111, then wait until the last cell output showing the public URL, e.g:
   ```
   Running on public URL: https://xxxxxxxxxxxxxxxxx.gradio.live
   ```

3. (Optional) Run [zip_outputs.ipynb](zip_outputs.ipynb) to zip outputs

4. (Optional) Download ouputs using the file manager panel (top icon) on the Paperspace left menu:
    1. Refresh the file manager
    2. Right click on the generated zip file insiden the outputs folder, e.g. `/outputs/outputs_20230519233742.zip`
    3. Select the option Download

5. (Optional) Run [delete_outputs.ipynb](delete_outputs.ipynb) to delete outputs

## Usage (Using Terminal)
Useful when Notebook is not working properly or there is an issue from Paperspace server
1. Open [Paperspace terminal](https://docs.paperspace.com/gradient/notebooks/terminal/)
2. Run this command:
    ```
    cd /notebooks/stable-diffusion-webui
    !python3 launch.py --enable-insecure-extension-access --share --gradio-auth admin:admin --precision full --no-half --xformers --disable-safe-unpickle
    ```
3. Wait until the terminal output showing the public URL, e.g:
   ```
   Running on public URL: https://xxxxxxxxxxxxxxxxx.gradio.live
   ```