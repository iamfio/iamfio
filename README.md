```typescript
interface Goal {
  name: string;
}

interface Skill extends Goal {
  level: 1 | 2 | 3 | 4 | 5;
}

class Me {
  public name = "Fiodor Go";
  public handle = "IamFio";
  private hobbies = [
    "Create Music",
    "Travel",
    "Reading Books",
    "Learning New Skills",
    "Bicycle",
    "Photography",
  ];
}

class AboutMe extends Me {
  private goals: Goal[];

  public getCurrentSkills(): Skill[] {
    return [
      { name: "JavaScript", level: 4 },
      { name: "TypeScript", level: 3 },
      { name: "React", level: 3 },
      { name: "Next 13", level: 3 },
      { name: "Vue 3", level: 2 },
      { name: "CSS", level: 4 },
      { name: "TailwindCSS", level: 3 },
      { name: "Bootstrap", level: 4 },
      { name: "MongoDB", level: 3 },
      { name: "Express", level: 3 },
      { name: "NestJS", level: 2 },
      { name: "PHP", level: 3 },
      { name: "Symfony", level: 3 },
      { name: "MySQL", level: 3 },
      { name: "Docker", level: 2 },
    ];
  }

  public getFutureGoals(): Goal[] {
    return [
      { name: "Go" },
      { name: "Angular" },
      { name: "Nuxt" },
      { name: "Develop and refine existing skills" },
    ];
  }
  
  public isOpenForNewJob(): boolean {
    return true;
  }
}


```
