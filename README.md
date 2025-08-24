# 👨‍💻 React Profile Card  

A simple **React.js project** that displays a profile card with an avatar, an introduction, and a dynamic list of skills.  
Great for practicing **components, props, lists, and conditional rendering** in React.  

---

## 🚀 Features  
- 📸 **Avatar** image of the user  
- 👋 **Introduction** with name and short bio  
- 🛠️ **Skills section** generated from an array  
- 🎨 Custom background colors for each skill  
- ⚡ Conditional rendering of emojis (👶 Beginner, 👍 Intermediate, 💪 Advanced)  

---

## 🛠️ Technologies Used  
- **React.js** (with Create React App)  
- **JavaScript (ES6+)**  
- **CSS3**  

---

## 💡 How It Works  
1. The **`App`** component renders the profile card.  
2. **`Avatar`** shows your image.  
3. **`Intro`** contains your name and description.  
4. **`SkillList`** maps over the `skills` array and renders multiple **`Skill`** components.  
5. Each **`Skill`** has:  
   - A `skill` name  
   - A `color` for background styling  
   - A `level` which shows an emoji (`👶 / 👍 / 💪`) depending on the value  

---

## 📂 Example Code  

```jsx
const skills = [
  { skill: "HTML + CSS", level: "advanced", color: "#2662EA" },
  { skill: "JavaScript", level: "advanced", color: "#EFDB1D" },
  { skill: "Git and Github", level: "intermediate", color: "#E84F33" },
  { skill: "React", level: "beginer", color: "#FF3B00" },
];

function Skill({ skill, color, level }) {
  return (
    <div className="skill" style={{ backgroundColor: color }}>
      <span>{skill}</span>
      <span>
        {level === "beginer" && "👶"}
        {level === "intermediate" && "👍"}
        {level === "advanced" && "💪"}
      </span>
    </div>
  );
}

---

## 🌐 Live Demo
👉 [View on GitHub Pages](https://your-username.github.io/react-profile-card/)

---

## 👨‍💻 Author
**Muhammad Muzammil Ijaz** – Frontend Developer 🚀  

