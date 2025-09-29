# Smart Research Intelligence Platform (SRIP)

Multi-agent business intelligence system delivering comprehensive market analysis, competitive positioning, and strategic recommendations for enterprise decision-making.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-HuggingFace_Spaces-blue?style=for-the-badge)](https://huggingface.co/spaces/Eshaal-Z/SRIP-platform)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg?style=for-the-badge)](https://www.python.org/downloads/)
[![LangGraph](https://img.shields.io/badge/🦜_LangGraph-Multi--Agent-green?style=for-the-badge)](https://github.com/langchain-ai/langgraph)

## Overview

SRIP transforms business intelligence through four specialized AI agents that conduct comprehensive market research, competitive analysis, and strategic planning. Built with LangGraph orchestration and optimized for enterprise deployment, the system delivers executive-ready reports in under 60 seconds.

### Key Capabilities

- **Market Intelligence**: Industry trends, market sizing, growth opportunities
- **Competitive Analysis**: Positioning assessment, competitive landscape mapping
- **Risk Evaluation**: Quantified risk scoring with mitigation strategies  
- **Strategic Advisory**: Executive recommendations and action planning

## Architecture

### Multi-Agent System Design

![SRIP Architecture](https://raw.githubusercontent.com/E-Z1937/SRIP-Platform/main/architecture-diagram.svg)

The system orchestrates four specialized agents through LangGraph:

| Agent | Function | Output |
|-------|----------|--------|
| **Market Intelligence Agent** | Industry analysis, market trends, growth projections | Market size, drivers, opportunities |
| **Competitive Intelligence Agent** | Competitive positioning, landscape mapping | Market share, advantages, vulnerabilities |
| **Risk Assessment Agent** | Strategic risk evaluation with 1-10 scoring | Quantified risks, mitigation strategies |
| **Strategic Advisor Agent** | Executive recommendations, action planning | 6-8 strategic recommendations, executive summary |

### Technical Stack

- **Orchestration**: LangGraph for agent coordination
- **LLM Integration**: Groq API with multi-model fallbacks
- **Interface**: Gradio web application
- **Deployment**: Hugging Face Spaces cloud hosting

## Performance Metrics

Based on production testing:

- **Processing Time**: 15-90 seconds for complete analysis
- **Success Rate**: 100% quality score capability
- **Content Delivery**: 5/5 sections completed consistently
- **Strategic Output**: 6-8 actionable recommendations per analysis

## Quick Start

### 1. Environment Setup

```bash
git clone https://github.com/E-Z1937/SRIP-Platform.git
cd SRIP-Platform

python -m venv srip-env
source srip-env/bin/activate  # Windows: srip-env\Scripts\activate

pip install -r requirements.txt
```

### 2. Configuration

Create `.env` file with your Groq API key:
```env
GROQ_API_KEY=your_groq_api_key_here
```

Get free API key at [console.groq.com](https://console.groq.com) (14,400 requests/day free tier)

### 3. Launch

```bash
python app.py
# Access at http://localhost:7860
```

## Usage Examples

### Cloud Infrastructure Analysis
```
Query: "Strategic analysis of cloud computing infrastructure market"
Targets: "AWS, Microsoft Azure, Google Cloud"

Results:
- Market size: $1.1 trillion by 2025 (31.4% CAGR)
- 8 strategic recommendations
- Risk assessment with quantified scores
- Executive summary with implementation plan
```

### AI Software Tools Analysis  
```
Query: "Competitive landscape for AI coding assistants"
Targets: "GitHub Copilot, OpenAI Codex, Amazon CodeWhisperer"

Results:
- Competitive positioning matrix
- Market share insights
- Strategic advantages/vulnerabilities
- Investment recommendations
```

## Project Structure

```
SRIP-Platform/
├── app.py                 # Main application
├── requirements.txt       # Dependencies
├── README.md             # This file
└── .env.example          # Environment template
```

## Deployment Options

### Local Development
```bash
python app.py
```

### Cloud Deployment
- **Hugging Face Spaces** (current): [Live Demo](https://huggingface.co/spaces/Eshaal-Z/SRIP-platform)
- **Railway/Render**: One-click deployment
- **Docker**: Container deployment ready

## Technical Features

### Agent Orchestration
- LangGraph workflow management
- Sequential processing with context sharing
- Multi-model fallback (llama-3.1-70b-versatile → mixtral-8x7b-32768 → llama-3.1-8b-instant)
- Comprehensive error handling

### Quality Assurance
- Content completeness validation
- Confidence scoring system
- Evidence-based analysis prompting
- Professional report formatting

### Performance Optimization
- Intelligent response caching
- Rate limit handling with progressive backoff
- Parallel-ready architecture
- Real-time processing status

## Real-World Applications

### Business Intelligence
- Strategic planning support
- Market entry analysis
- Competitive positioning
- Investment research

### Enterprise Use Cases
- Due diligence for M&A
- Product strategy development
- Risk management planning
- Competitive response strategies

## Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/enhancement`)
3. Test changes thoroughly
4. Submit pull request with description

## API Reference

### Core Analysis Function
```python
def execute_complete_analysis(query: str, targets: str) -> Tuple[str, str]:
    """
    Run comprehensive business intelligence analysis
    
    Args:
        query: Strategic research question
        targets: Comma-separated analysis focus areas
        
    Returns:
        (formatted_report, status_message)
    """
```

## System Requirements

- Python 3.11+
- Internet connection for API calls
- Groq API key (free tier sufficient)
- 2GB RAM minimum for local deployment

## Troubleshooting

### Common Issues

**API Key Error**
```bash
# Verify environment variable is set
echo $GROQ_API_KEY
```

**Processing Timeout**
- Check internet connection
- Verify API key validity
- Retry with simpler query

**Quality Issues** 
- Ensure query is business-focused and specific
- Provide clear analysis targets when possible
- Review example queries for optimal formatting

## License

MIT License - see LICENSE file for details.

## Built With

- [LangGraph](https://github.com/langchain-ai/langgraph) - Multi-agent orchestration
- [Groq](https://groq.com/) - High-performance LLM inference
- [Gradio](https://gradio.app/) - Web interface framework
- [Hugging Face Spaces](https://huggingface.co/spaces) - Cloud deployment

---
 
**Live Demo**: https://huggingface.co/spaces/Eshaal-Z/SRIP-platform
