# UserSecrets App
Mały program pokazujący zastosowanie User Secretów /n

## Tworzenie User Secreta
Aby utworzyć User Secreta pierwszym krokiem należy postąpić wedłu jednej z poniższych metod:
* Otworzyć terminal, następnie przenieść się do folderu z plikiem UserAPI.csproj, następnie wprowadzić komendę **dotnet user-secrets init**
* W edytorze (np. VS Code) otworzyć plik UserAPI.csproj a nstępnie wewnątrz tagów PropertyGroup utworzyć nowy zestaw tagów **<UserSecretsId></UserSecretsId>** wewnątrz którego należy umieścić secret przy użyciu np. insert GUID. Warto również dodać prefix ułatwiający odszukanie właściwego secreta w razie potrzeby

## Tworzenie klucza (na przykładzie hasła) z użyciem User Secreta
Aby utworzyć hasło z wykorzystaniem User Secreta należy w terminalu przenieść się do folderu w którym znajduje się plik UserAPI.csproj a następnie wprowadzić komendę **dotnet user-secrets set "Password" "jakiestamhaslo"**