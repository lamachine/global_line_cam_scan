# global_line_cam_scan
Use arducam to scan a line and produce a 3d graph
  Need to add odometer of some sort for distance between lines
  https://www.youtube.com/watch?v=l0KUXxfalIQ
  Use my robot for now
  Buy a cheap RC car?

Hook up the cam
  https://docs.arducam.com/Raspberry-Pi-Camera/Native-camera/Quick-Start-Guide/

Scan the line by color

Best fit line
  https://www.statology.org/line-of-best-fit-python/
    #find line of best fit
    a, b = np.polyfit(x, y, 1)
    
    #add points to plot
    plt.scatter(x, y)
    
    #add line of best fit to plot
    plt.plot(x, a*x+b)

Calculate deviations from average line

Set limits on what is interesting
  Max deviation
  Missing information
  Possibly curves (post processing)
  Possibly slope (post processing)
  
Set alerts from these limits
