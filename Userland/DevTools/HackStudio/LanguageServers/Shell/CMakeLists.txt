serenity_component(
    ShellLanguageServer
    TARGETS ShellLanguageServer
)

set(SOURCES
    ShellComprehensionEngine.cpp
    main.cpp
)

set(GENERATED_SOURCES
    ../LanguageServerEndpoint.h
    ../LanguageClientEndpoint.h)

serenity_bin(ShellLanguageServer)

# We link with LibGUI because we use GUI::TextDocument to update
# the content of files according to the edit actions we receive over IPC.
target_link_libraries(ShellLanguageServer LibIPC LibShell LibGUI LibLanguageServer LibMain)
