### You are a senior .NET architect tasked with migrating an existing WCF service project to ASP.NET Web API 2 (targeting .NET Framework 4.7.2) using Visual Studio 2022/2026.

### Source Project Path:  
C:\Users\india\OneDrive\FromYourPhone\Desktop\Antigravity-Demo-4\SchoolServiceSoap\SchoolService.sln

### Target Project Path (blank Web API solution):  
C:\Users\india\OneDrive\FromYourPhone\Desktop\Antigravity-Demo-4\SchoolServiceRest\SchoolServiceRest\SchoolServiceRest.slnx

Your task is to help me convert this code into a clean, modern Web API following best practices.

### Requirements:
1. Convert WCF services (ServiceContract, OperationContract) into RESTful API controllers.
2. Use the C# programming language
3. Replace SOAP-based structure with HTTP-based routing (GET, POST, PUT, DELETE).
4. Preserve existing business logic but refactor where needed for better separation of concerns.
5. Move logic into:
   - Controllers (thin layer)
   - Services (business logic)
   - DTOs / Models
6. Convert DataContracts/DataMembers into standard C# models.
7. Transform validation logic:
   - Existing custom validation → FluentValidation or Data Annotations
8. Handle exception handling properly using middleware or filters.
9. Replace WCF configuration (web.config) with appsettings.json and dependency injection.
10. Ensure async/await usage where applicable.
11. Suggest improvements:
    - Dependency Injection
    - Logging (ILogger)
    - Clean architecture (if possible)
    - API versioning (optional)
12. Preserve backward compatibility considerations if needed.

### Input:
I will provide:
- WCF service interface(s)
- Implementation classes
- Validation methods
- DTOs / DataContracts

### Output format:
For each input:
1. Converted API Controller
2. Service interface + implementation
3. Updated Model/DTO
4. Validation approach
5. Notes on improvements or refactoring

### Additional expectations:
- Avoid over-engineering but follow modern .NET best practices
- Keep code clean, readable, and production-ready
- Highlight any breaking changes from WCF to Web API
- If something cannot be directly translated, propose an equivalent design
- Once the migration is complete, please build with VS2022 or VS2026, run the rest of the project, test all REST APIs, and capture the result in a document.

### Additional Instructions
- During migration, if you encounter issues restoring NuGet packages due to an Internet proxy, please skip them for now. Instead, create a document listing those packages so we can download them later and reference them in our project.
- Do not connect to, or execute any SQL queries against, SQL Server, Oracle, or any other database.
