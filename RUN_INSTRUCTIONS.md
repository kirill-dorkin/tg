# Инструкция по запуску проекта

1. **Установите инструменты для сборки .NET Framework 4.8**
   - Нужна система Windows с установленным .NET Framework 4.8.
   - Проще всего использовать Visual Studio 2019/2022 с рабочей нагрузкой "*.NET desktop development*" или Build Tools for Visual Studio.

2. **Клонируйте репозиторий**
   ```bash
   git clone <URL_репозитория>
   cd tg
   ```

3. **Восстановите NuGet-пакеты**
   ```bash
   nuget restore TgApp.sln
   ```

4. **Соберите проект**
   ```bash
   msbuild TgApp.sln
   ```

5. **Запустите приложение**
   После сборки исполняемый файл появится в `TgApp\bin\Debug\TgApp.exe` (или в `bin\Release` для сборки Release).
   Запустите его двойным кликом или из командной строки:
   ```bash
   cd TgApp/bin/Debug
   TgApp.exe
   ```

Приложение откроет графический интерфейс, через который можно пользоваться функционалом, описанным в README.
