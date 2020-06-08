FROM nanquitas/vscode/devkitarm:latest

# Download 3gxtool
# This is temporary, when the new 3gx format and the 3gx api is ready, a proper repo will be created
RUN cd home \
    && wget https://cdn.discordapp.com/attachments/463776354899460101/718621100665208842/3gxtool \
    && mv ./3gxtool ${DEVKITPRO}/tools/bin/3gxtool \
    && chmod +x ${DEVKITPRO}/tools/bin/3gxtool
