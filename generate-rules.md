Create four LangGPT-style code generation rule files in the `@instructions` directory. Each file should follow the LangGPT format with Role, Profile, Rules, Goals, Constraints, Workflows, and Initialization sections. Generate the following files:

1. **generate-biz-component.md**: Business component generation rules
   - **Output files**: 
     - `index.ts` (component exports)
     - `interface.ts` (TypeScript interfaces and types)
     - `[ComponentName].stories.tsx` (Storybook stories)
     - `[ComponentName].tsx` (main React component)
   - **Requirements**: Follow modern React patterns, include proper TypeScript typing, and Storybook integration

2. **generate-model-repository.md**: Data layer generation rules following Trevor Lasn's Three Layers pattern
   - **Step 0**: Analyze existing Prisma schema before code generation
   - **Output**: Prisma schema definitions and repository layer code
   - **Requirements**: Handle schema modifications cautiously, provide migration guidance, follow repository pattern

3. **generate-api-service.md**: API and service layer generation rules
   - **Output**: Next.js API routes and service layer code
   - **Requirements**: Include proper error handling, validation, and follow RESTful conventions

4. **generate-page-component.md**: Page component generation with data integration
   - **Architecture**: Follow Three-Layer Data Architecture pattern
     - Layer 1: Server Components (page.tsx) that integrate React Query hooks
     - Layer 2: React Query hooks that encapsulate data logic
     - Layer 3: UI components for user interactions
   - **Requirements**: 
     - Use React Query for client-side rendering
     - Include proper query keys hierarchy
     - Implement optimistic updates with rollback mechanisms
     - Configure appropriate staleTime/gcTime for performance
     - Integrate with API services and business components

Each rule file should be comprehensive, include specific examples, and follow consistent naming conventions and project structure patterns.
