# 🤖 Multi-Agent Sales Outreach System

An **AI-powered multi-agent system** that automates **lead profiling** and **personalized outreach** using [CrewAI](https://github.com/joaomdmoura/crewai).  

It simulates a **sales team** where specialized agents collaborate to identify high-value leads and craft tailored outreach campaigns.

## ✨ Features
- 🧑‍💼 **Sales Representative Agent** → Profiles potential leads, researches decision-makers, and identifies opportunities.  
- 📩 **Lead Sales Representative Agent** → Crafts personalized outreach campaigns tailored to leads’ recent achievements.  
- 🔍 **Integrated Tools**:  
  - Web Search (SerperDevTool)  
  - File & Directory Readers (to analyze internal instructions)  
  - Custom **Sentiment Analysis Tool** (ensures positive & engaging tone).  

## ⚙️ Workflow
1. **Lead Profiling Task** 🕵️‍♂️  
   - Gathers detailed insights on the company, key personnel, and business needs.  
   - Uses multiple tools for reliable data collection.  

2. **Personalized Outreach Task** ✍️  
   - Crafts compelling outreach emails targeting key decision-makers.  
   - Ensures messaging aligns with the company’s culture and milestones.  

3. **Crew Execution** 🛠️  
   - Agents collaborate within a `Crew`.  
   - Inputs like `lead_name`, `industry`, `decision_maker`, and `milestone` guide the workflow.  

## 📊 Example Run

```python
inputs = {
    "lead_name": "DeepLearningAI",
    "industry": "Online Learning Platform",
    "key_decision_maker": "Andrew Ng",
    "position": "CEO",
    "milestone": "product launch"
}

result = crew.kickoff(inputs=inputs)
print(result)
```

✅ Output:

A structured lead profiling report + personalized email drafts targeting the decision-maker.

## 🚀 Tech Stack

- Python
- CrewAI (multi-agent orchestration)
- CrewAI Tools (Search, File, Directory readers)
- Custom Tools (Sentiment Analysis)

## 🎯 Use Cases
- Automating sales lead generation
- Building personalized outreach campaigns at scale
- Showcasing multi-agent collaboration for business workflows

