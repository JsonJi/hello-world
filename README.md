# hello-world
hello-world测试1
@RequestMapping(value = "/toAdd")
    public ModelAndView toAdd(HttpServletRequest request){
        ModelAndView mv = new ModelAndView();
        mv.addObject("fence",new Fence());
        mv.setViewName("bdpt/fence/add");
        BackUrlUtil.setBackUrl(mv, request);// 设置返回的url
        return mv;
    }
