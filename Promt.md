You are a senior .NET architect.

I have an existing WCF service project that I want to migrate to ASP.NET Web API 2 (.NET Framework7.2) 
Visual Studio 2022 is installed on my Local Machine, Use Vissual studio to do the code and compile. 
The codebase is large and includes multiple service contracts, data contracts, business logic classes, and validation methods. 
I have selected the source Project as "C:\Users\RBarhgoojer\OneDrive - Colt Technology Services\Desktop\Antigravity-Demo-3\WCFSchoolService\SchoolService.sln" , 
I have already created Sample Propject ASP.NET Web API 2 (.NET Framework7.2)  ""C:\Users\RBarhgoojer\OneDrive - Colt Technology Services\Desktop\Antigravity-Demo-3\RestSchoolService\RestSchoolService\RestSchoolService.sln"", In this Project i have to migrated my wcf Project

Your task is to help me convert this code into a clean, modern Web API following best practices.

### Requirements:
1. Convert WCF services (ServiceContract, OperationContract) into RESTful API controllers.
2. Replace SOAP-based structure with HTTP-based routing (GET, POST, PUT, DELETE).
3. Preserve existing business logic but refactor where needed for better separation of concerns.
4. Move logic into:
   - Controllers (thin layer)
   - Services (business logic)
   - DTOs / Models
5. Convert DataContracts/DataMembers into standard C# models.
6. Transform validation logic:
   - Existing custom validation → FluentValidation or Data Annotations
7. Handle exception handling properly using middleware or filters.
8. Replace WCF configuration (web.config) with appsettings.json and dependency injection.
9. Ensure async/await usage where applicable.
10. Suggest improvements:
    - Dependency Injection
    - Logging (ILogger)
    - Clean architecture (if possible)
    - API versioning (optional)
11. Preserve backward compatibility considerations if needed.

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
- Once migration done Please build and run the rest Project and test All Rest APIs and capture the result in doucment

### Additional Instruction
- During Migration if you get isssue to restore nuget pagcages due to Internet Proxy then Please leave them but make doucment for us that we can download later and refernece them in our Project 
