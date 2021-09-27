# phase-0
08049581 <phase_0>:
 8049581:	f3 0f 1e fb          	endbr32 
 8049585:	55                   	push   %ebp
 8049586:	89 e5                	mov    %esp,%ebp
 8049588:	83 ec 08             	sub    $0x8,%esp
 804958b:	83 ec 08             	sub    $0x8,%esp
 804958e:	68 ec b1 04 08       	push   $0x804b1ec
 8049593:	ff 75 08             	pushl  0x8(%ebp)
 8049596:	e8 11 08 00 00       	call   8049dac <strings_not_equal>
 804959b:	83 c4 10             	add    $0x10,%esp
 804959e:	85 c0                	test   %eax,%eax
 80495a0:	74 0c                	je     80495ae <phase_0+0x2d>
 80495a2:	e8 85 0a 00 00       	call   804a02c <explode_bomb>
 80495a7:	b8 00 00 00 00       	mov    $0x0,%eax
 80495ac:	eb 05                	jmp    80495b3 <phase_0+0x32>
 80495ae:	b8 01 00 00 00       	mov    $0x1,%eax
 80495b3:	c9                   	leave  
 80495b4:	c3                   	ret    
