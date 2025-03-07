
# react-vertical-timeline-revamped

A modern React vertical timeline component. This package is a revamped version of the original [react-vertical-timeline-component](https://github.com/stephane-monnot/react-vertical-timeline) by Stephane Monnot.

## Why This Fork?

The original package is no longer actively maintained. I needed to use this component with modern React applications but couldn't update all the original code right away. This revamped version aims to:

- Support the latest React versions
- Provide TypeScript typings
- Maintain the same API for a seamless transition

**Note:** The usage is exactly the same as the original component from Stephane Monnot. Future updates will include improved documentation and tests to meet current standards.

## Installation

npm install react-vertical-timeline-revamped

or

yarn add react-vertical-timeline-revamped

## Usage

The usage is identical to the original component:

```
---
import { VerticalTimeline, VerticalTimelineElement }  from 'react-vertical-timeline-revamped';

...

<VerticalTimeline>
  <VerticalTimelineElement
    className="vertical-timeline-element--work"
    contentStyle={{ background: 'rgb(33, 150, 243)', color: '#fff' }}
    contentArrowStyle={{ borderRight: '7px solid  rgb(33, 150, 243)' }}
    date="2011 - present"
    iconStyle={{ background: 'rgb(33, 150, 243)', color: '#fff' }}
    icon={<WorkIcon />}
  >
    <h3 className="vertical-timeline-element-title">Creative Director</h3>
    <h4 className="vertical-timeline-element-subtitle">Miami, FL</h4>
    <p>
      Creative Direction, User Experience, Visual Design, Project Management, Team Leading
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    className="vertical-timeline-element--work"
    date="2010 - 2011"
    iconStyle={{ background: 'rgb(33, 150, 243)', color: '#fff' }}
    icon={<WorkIcon />}
  >
    <h3 className="vertical-timeline-element-title">Art Director</h3>
    <h4 className="vertical-timeline-element-subtitle">San Francisco, CA</h4>
    <p>
      Creative Direction, User Experience, Visual Design, SEO, Online Marketing
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    className="vertical-timeline-element--work"
    date="2008 - 2010"
    iconStyle={{ background: 'rgb(33, 150, 243)', color: '#fff' }}
    icon={<WorkIcon />}
  >
    <h3 className="vertical-timeline-element-title">Web Designer</h3>
    <h4 className="vertical-timeline-element-subtitle">Los Angeles, CA</h4>
    <p>
      User Experience, Visual Design
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    className="vertical-timeline-element--work"
    date="2006 - 2008"
    iconStyle={{ background: 'rgb(33, 150, 243)', color: '#fff' }}
    icon={<WorkIcon />}
  >
    <h3 className="vertical-timeline-element-title">Web Designer</h3>
    <h4 className="vertical-timeline-element-subtitle">San Francisco, CA</h4>
    <p>
      User Experience, Visual Design
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    className="vertical-timeline-element--education"
    date="April 2013"
    iconStyle={{ background: 'rgb(233, 30, 99)', color: '#fff' }}
    icon={<SchoolIcon />}
  >
    <h3 className="vertical-timeline-element-title">Content Marketing for Web, Mobile and Social Media</h3>
    <h4 className="vertical-timeline-element-subtitle">Online Course</h4>
    <p>
      Strategy, Social Media
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    className="vertical-timeline-element--education"
    date="November 2012"
    iconStyle={{ background: 'rgb(233, 30, 99)', color: '#fff' }}
    icon={<SchoolIcon />}
  >
    <h3 className="vertical-timeline-element-title">Agile Development Scrum Master</h3>
    <h4 className="vertical-timeline-element-subtitle">Certification</h4>
    <p>
      Creative Direction, User Experience, Visual Design
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    className="vertical-timeline-element--education"
    date="2002 - 2006"
    iconStyle={{ background: 'rgb(233, 30, 99)', color: '#fff' }}
    icon={<SchoolIcon />}
  >
    <h3 className="vertical-timeline-element-title">Bachelor of Science in Interactive Digital Media Visual Imaging</h3>
    <h4 className="vertical-timeline-element-subtitle">Bachelor Degree</h4>
    <p>
      Creative Direction, Visual Design
    </p>
  </VerticalTimelineElement>
  <VerticalTimelineElement
    iconStyle={{ background: 'rgb(16, 204, 82)', color: '#fff' }}
    icon={<StarIcon />}
  />
</VerticalTimeline>

```

**Note:** notice that importing 'react-vertical-timeline-revamped/dist/style.min.css' is not needed anymore


## Props

### VerticalTimeline Props

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| animate | Boolean | true | Enable or disable animations on elements |
| className | String | | Add extra class name to root div element |
| layout | String | '2-columns' | Choose layout: '1-column-left', '1-column-right', or '2-columns' |
| lineColor | String | 'white' | Choose a color for the timeline |

### VerticalTimelineElement Props

| Prop | Type | Description |
|------|------|-------------|
| date | String | Date of the element |
| iconStyle | Object | Style of the element's icon |
| icon | ReactNode | Icon of the element |
| position | String | Position of the element (left or right) |
| contentStyle | Object | Style of the content container |
| contentArrowStyle | Object | Style of the content arrow |
| className | String | Additional CSS class for the element |
| dateClassName | String | Add extra class name to the element's date |
| iconClassName | String | Add extra class name to the element's icon |
| shadowSize | String | Shadow size for icon (default: 'small'). Available sizes are 'small', 'medium' and 'large' |
| iconOnClick | Function | onClick handler of the element's icon |
| onTimelineElementClick | Function | onClick handler of the vertical timeline element's div |
| style | Object | Add extra style to root div element |
| textClassName | String | Add extra class name to the text container |
| intersectionObserverProps | Object | Custom props pass to useInView component (default: { rootMargin: '0px 0px 40px 0px' }). See react-intersection-observer for more information |
| visible | Boolean | Show element by default even if it is outside of the viewport (default: false) |


## Future Plans

- Update documentation
- Add comprehensive test suite
- Improve TypeScript definitions
- Enhance accessibility

## Credits

This package is based on [react-vertical-timeline-component](https://github.com/stephane-monnot/react-vertical-timeline) by Stephane Monnot, which is licensed under MIT.

## License

MIT License